# Comparing `tmp/fern_merge-0.0.28.tar.gz` & `tmp/fern_merge-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_merge-0.0.28.tar", max compression
+gzip compressed data, was "fern_merge-0.0.29.tar", max compression
```

## Comparing `fern_merge-0.0.28.tar` & `fern_merge-0.0.29.tar`

### file list

```diff
@@ -1,421 +1,455 @@
--rw-r--r--   0        0        0     2139 2023-07-12 19:36:44.472510 fern_merge-0.0.28/README.md
--rw-r--r--   0        0        0      371 2023-07-12 19:36:44.472510 fern_merge-0.0.28/pyproject.toml
--rw-r--r--   0        0        0      187 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/__init__.py
--rw-r--r--   0        0        0     1547 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/client.py
--rw-r--r--   0        0        0      528 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/api_error.py
--rw-r--r--   0        0        0     1101 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      201 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/environment.py
--rw-r--r--   0        0        0        0 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/py.typed
--rw-r--r--   0        0        0      116 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/__init__.py
--rw-r--r--   0        0        0     8926 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/__init__.py
--rw-r--r--   0        0        0    10018 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/client.py
--rw-r--r--   0        0        0     1144 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2284 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/activities/__init__.py
--rw-r--r--   0        0        0    12088 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/activities/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/applications/__init__.py
--rw-r--r--   0        0        0    14581 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/applications/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/__init__.py
--rw-r--r--   0        0        0    11850 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2304 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/__init__.py
--rw-r--r--   0        0        0    16506 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2045 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/departments/__init__.py
--rw-r--r--   0        0        0     5972 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/departments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/__init__.py
--rw-r--r--   0        0        0     8117 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2362 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2537 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/__init__.py
--rw-r--r--   0        0        0    12540 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/issues/__init__.py
--rw-r--r--   0        0        0     6768 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/__init__.py
--rw-r--r--   0        0        0     6771 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/__init__.py
--rw-r--r--   0        0        0     8227 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4774 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5305 2023-07-12 19:36:44.472510 fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offers/__init__.py
--rw-r--r--   0        0        0     8095 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offers/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offices/__init__.py
--rw-r--r--   0        0        0     5900 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/offices/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4816 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2545 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/__init__.py
--rw-r--r--   0        0        0     6014 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/__init__.py
--rw-r--r--   0        0        0     8545 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6892 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2644 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/tags/__init__.py
--rw-r--r--   0        0        0     4201 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/users/__init__.py
--rw-r--r--   0        0        0     7399 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/users/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4191 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    12298 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/__init__.py
--rw-r--r--   0        0        0     1240 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/access_role_enum.py
--rw-r--r--   0        0        0     1483 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/account_token.py
--rw-r--r--   0        0        0      857 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_remote_fields.py
--rw-r--r--   0        0        0      869 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      873 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      885 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     2693 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity.py
--rw-r--r--   0        0        0      189 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_activity_type.py
--rw-r--r--   0        0        0     2121 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_request.py
--rw-r--r--   0        0        0      196 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_request_activity_type.py
--rw-r--r--   0        0        0     1109 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_response.py
--rw-r--r--   0        0        0      705 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/activity_type_enum.py
--rw-r--r--   0        0        0     2473 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application.py
--rw-r--r--   0        0        0     2269 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application_request.py
--rw-r--r--   0        0        0     1121 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/application_response.py
--rw-r--r--   0        0        0     8243 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/applications_list_request_expand.py
--rw-r--r--   0        0        0     8371 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/applications_retrieve_request_expand.py
--rw-r--r--   0        0        0     2146 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment.py
--rw-r--r--   0        0        0      199 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_attachment_type.py
--rw-r--r--   0        0        0     1820 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request.py
--rw-r--r--   0        0        0      206 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request_attachment_type.py
--rw-r--r--   0        0        0     1117 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_response.py
--rw-r--r--   0        0        0      985 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/attachment_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/available_actions.py
--rw-r--r--   0        0        0     3471 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate.py
--rw-r--r--   0        0        0     3061 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate_request.py
--rw-r--r--   0        0        0     1113 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidate_response.py
--rw-r--r--   0        0        0      833 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidates_list_request_expand.py
--rw-r--r--   0        0        0      849 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
--rw-r--r--   0        0        0     1391 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     2324 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/condition_type_enum.py
--rw-r--r--   0        0        0      870 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     1698 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/department.py
--rw-r--r--   0        0        0     1337 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/disability_status_enum.py
--rw-r--r--   0        0        0     4088 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeoc.py
--rw-r--r--   0        0        0     3803 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
--rw-r--r--   0        0        0     3851 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     3867 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     3915 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1529 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address.py
--rw-r--r--   0        0        0      210 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_email_address_type.py
--rw-r--r--   0        0        0     1553 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request.py
--rw-r--r--   0        0        0      217 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request_email_address_type.py
--rw-r--r--   0        0        0      742 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/email_address_type_enum.py
--rw-r--r--   0        0        0      522 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/error_validation_problem.py
--rw-r--r--   0        0        0     1160 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/gender_enum.py
--rw-r--r--   0        0        0     4187 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/interviews_list_request_expand.py
--rw-r--r--   0        0        0     4251 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
--rw-r--r--   0        0        0     1336 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issue.py
--rw-r--r--   0        0        0      555 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/issues_list_request_status.py
--rw-r--r--   0        0        0     3441 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job.py
--rw-r--r--   0        0        0     2387 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job_interview_stage.py
--rw-r--r--   0        0        0     1045 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/job_status_enum.py
--rw-r--r--   0        0        0     3771 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_expand.py
--rw-r--r--   0        0        0      956 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_status.py
--rw-r--r--   0        0        0     3835 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
--rw-r--r--   0        0        0      835 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-12 19:36:44.476511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0     1037 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/model_operation.py
--rw-r--r--   0        0        0     1946 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/multipart_form_field_request.py
--rw-r--r--   0        0        0     2799 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offer.py
--rw-r--r--   0        0        0     1832 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offer_status_enum.py
--rw-r--r--   0        0        0      767 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offers_list_request_expand.py
--rw-r--r--   0        0        0      783 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/offers_retrieve_request_expand.py
--rw-r--r--   0        0        0     1817 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/office.py
--rw-r--r--   0        0        0      993 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/operator_schema.py
--rw-r--r--   0        0        0     1180 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/overall_recommendation_enum.py
--rw-r--r--   0        0        0      959 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      892 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_activity_list.py
--rw-r--r--   0        0        0      904 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_application_list.py
--rw-r--r--   0        0        0      900 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_attachment_list.py
--rw-r--r--   0        0        0      896 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_candidate_list.py
--rw-r--r--   0        0        0      921 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      900 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_department_list.py
--rw-r--r--   0        0        0      876 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_eeoc_list.py
--rw-r--r--   0        0        0      880 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_issue_list.py
--rw-r--r--   0        0        0      930 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
--rw-r--r--   0        0        0      872 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_list.py
--rw-r--r--   0        0        0      880 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_offer_list.py
--rw-r--r--   0        0        0      884 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_office_list.py
--rw-r--r--   0        0        0      909 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_reject_reason_list.py
--rw-r--r--   0        0        0      901 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_remote_user_list.py
--rw-r--r--   0        0        0      933 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
--rw-r--r--   0        0        0      896 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scorecard_list.py
--rw-r--r--   0        0        0      901 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      872 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/paginated_tag_list.py
--rw-r--r--   0        0        0     3068 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/patched_candidate_request.py
--rw-r--r--   0        0        0     1624 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number.py
--rw-r--r--   0        0        0      205 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_phone_number_type.py
--rw-r--r--   0        0        0     1648 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_request.py
--rw-r--r--   0        0        0      212 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
--rw-r--r--   0        0        0     1039 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_type_enum.py
--rw-r--r--   0        0        0     2326 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/race_enum.py
--rw-r--r--   0        0        0      814 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/reason_enum.py
--rw-r--r--   0        0        0     1775 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/reject_reason.py
--rw-r--r--   0        0        0      802 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_response_response_type.py
--rw-r--r--   0        0        0     2543 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/remote_user.py
--rw-r--r--   0        0        0      723 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/request_format_enum.py
--rw-r--r--   0        0        0      562 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/response_type_enum.py
--rw-r--r--   0        0        0     3200 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview.py
--rw-r--r--   0        0        0     2455 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_request.py
--rw-r--r--   0        0        0     1150 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_response.py
--rw-r--r--   0        0        0      893 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_status_enum.py
--rw-r--r--   0        0        0     2677 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecard.py
--rw-r--r--   0        0        0     1731 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_list_request_expand.py
--rw-r--r--   0        0        0     1763 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
--rw-r--r--   0        0        0      695 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1623 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/tag.py
--rw-r--r--   0        0        0     1659 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url.py
--rw-r--r--   0        0        0     1683 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_request.py
--rw-r--r--   0        0        0      171 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_request_url_type.py
--rw-r--r--   0        0        0     1451 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_type_enum.py
--rw-r--r--   0        0        0      164 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/url_url_type.py
--rw-r--r--   0        0        0      762 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/validation_problem_source.py
--rw-r--r--   0        0        0     1467 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/veteran_status_enum.py
--rw-r--r--   0        0        0      760 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/visibility_enum.py
--rw-r--r--   0        0        0      915 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/ats/types/webhook_receiver.py
--rw-r--r--   0        0        0     9130 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/__init__.py
--rw-r--r--   0        0        0     9511 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/client.py
--rw-r--r--   0        0        0     1106 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/__init__.py
--rw-r--r--   0        0        0     2286 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/__init__.py
--rw-r--r--   0        0        0     2306 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/__init__.py
--rw-r--r--   0        0        0     8705 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/__init__.py
--rw-r--r--   0        0        0     6633 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/companies/__init__.py
--rw-r--r--   0        0        0     5928 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/companies/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
--rw-r--r--   0        0        0     8024 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employees/__init__.py
--rw-r--r--   0        0        0    17328 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employees/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employments/__init__.py
--rw-r--r--   0        0        0     8741 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/employments/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/__init__.py
--rw-r--r--   0        0        0     2539 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/groups/__init__.py
--rw-r--r--   0        0        0     7291 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/issues/__init__.py
--rw-r--r--   0        0        0     6772 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/issues/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/__init__.py
--rw-r--r--   0        0        0     4776 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/__init__.py
--rw-r--r--   0        0        0     5307 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/locations/__init__.py
--rw-r--r--   0        0        0     7265 2023-07-12 19:36:44.480511 fern_merge-0.0.28/src/merge/resources/hris/resources/locations/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/__init__.py
--rw-r--r--   0        0        0     4818 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/__init__.py
--rw-r--r--   0        0        0     5946 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/__init__.py
--rw-r--r--   0        0        0     8756 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/__init__.py
--rw-r--r--   0        0        0     2547 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/__init__.py
--rw-r--r--   0        0        0     6898 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/__init__.py
--rw-r--r--   0        0        0     2646 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/teams/__init__.py
--rw-r--r--   0        0        0     6609 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/teams/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/__init__.py
--rw-r--r--   0        0        0    12810 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/__init__.py
--rw-r--r--   0        0        0     8364 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/client.py
--rw-r--r--   0        0        0       65 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/__init__.py
--rw-r--r--   0        0        0     4195 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/client.py
--rw-r--r--   0        0        0    12720 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details.py
--rw-r--r--   0        0        0     1900 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions.py
--rw-r--r--   0        0        0     1112 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_integration.py
--rw-r--r--   0        0        0      896 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
--rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_integration.py
--rw-r--r--   0        0        0      845 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_token.py
--rw-r--r--   0        0        0      555 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/account_type_enum.py
--rw-r--r--   0        0        0     1245 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/available_actions.py
--rw-r--r--   0        0        0     2399 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info.py
--rw-r--r--   0        0        0      185 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_account_type.py
--rw-r--r--   0        0        0      529 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_account_type.py
--rw-r--r--   0        0        0      728 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_order_by.py
--rw-r--r--   0        0        0     2342 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/benefit.py
--rw-r--r--   0        0        0     1391 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/categories_enum.py
--rw-r--r--   0        0        0     1375 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/category_enum.py
--rw-r--r--   0        0        0      997 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/common_model_scopes_body_request.py
--rw-r--r--   0        0        0     1962 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/company.py
--rw-r--r--   0        0        0     2324 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema.py
--rw-r--r--   0        0        0      200 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema_condition_type.py
--rw-r--r--   0        0        0     1478 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/condition_type_enum.py
--rw-r--r--   0        0        0    35178 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/country_enum.py
--rw-r--r--   0        0        0      870 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/debug_mode_log.py
--rw-r--r--   0        0        0      792 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/debug_model_log_summary.py
--rw-r--r--   0        0        0     2140 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/deduction.py
--rw-r--r--   0        0        0     2143 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning.py
--rw-r--r--   0        0        0      177 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning_type.py
--rw-r--r--   0        0        0      949 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/earning_type_enum.py
--rw-r--r--   0        0        0     6740 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee.py
--rw-r--r--   0        0        0     2796 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_run.py
--rw-r--r--   0        0        0      829 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
--rw-r--r--   0        0        0      845 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
--rw-r--r--   0        0        0     6116 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_request.py
--rw-r--r--   0        0        0     1109 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employee_response.py
--rw-r--r--   0        0        0      739 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_employment_status.py
--rw-r--r--   0        0        0    80247 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_expand.py
--rw-r--r--   0        0        0     4067 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_remote_fields.py
--rw-r--r--   0        0        0     4115 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
--rw-r--r--   0        0        0    81343 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_expand.py
--rw-r--r--   0        0        0     4131 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4179 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0    18610 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment.py
--rw-r--r--   0        0        0      199 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_employment_type.py
--rw-r--r--   0        0        0      770 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_status_enum.py
--rw-r--r--   0        0        0     1166 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employment_type_enum.py
--rw-r--r--   0        0        0      777 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_expand.py
--rw-r--r--   0        0        0      707 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_order_by.py
--rw-r--r--   0        0        0     4219 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_remote_fields.py
--rw-r--r--   0        0        0     4267 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      793 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_expand.py
--rw-r--r--   0        0        0     4283 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     4331 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0      522 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/enabled_actions_enum.py
--rw-r--r--   0        0        0      739 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/encoding_enum.py
--rw-r--r--   0        0        0      913 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/error_validation_problem.py
--rw-r--r--   0        0        0     2511 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/ethnicity_enum.py
--rw-r--r--   0        0        0      986 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/flsa_status_enum.py
--rw-r--r--   0        0        0     1146 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/gender_enum.py
--rw-r--r--   0        0        0     2225 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group.py
--rw-r--r--   0        0        0      169 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group_type.py
--rw-r--r--   0        0        0     1136 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/group_type_enum.py
--rw-r--r--   0        0        0     1336 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issue.py
--rw-r--r--   0        0        0      555 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issue_status_enum.py
--rw-r--r--   0        0        0      508 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/issues_list_request_status.py
--rw-r--r--   0        0        0      835 2023-07-12 19:36:44.484511 fern_merge-0.0.28/src/merge/resources/hris/types/link_token.py
--rw-r--r--   0        0        0     1488 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition.py
--rw-r--r--   0        0        0     1079 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition_request.py
--rw-r--r--   0        0        0      998 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
--rw-r--r--   0        0        0     1010 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
--rw-r--r--   0        0        0      799 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_status.py
--rw-r--r--   0        0        0     1354 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/linked_accounts_list_request_category.py
--rw-r--r--   0        0        0    11858 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location.py
--rw-r--r--   0        0        0      189 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location_location_type.py
--rw-r--r--   0        0        0      509 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/location_type_enum.py
--rw-r--r--   0        0        0     1685 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/marital_status_enum.py
--rw-r--r--   0        0        0     1037 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/meta_response.py
--rw-r--r--   0        0        0     1275 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/method_enum.py
--rw-r--r--   0        0        0     1162 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/model_operation.py
--rw-r--r--   0        0        0     1946 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/multipart_form_field_request.py
--rw-r--r--   0        0        0      993 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/operator_schema.py
--rw-r--r--   0        0        0      959 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
--rw-r--r--   0        0        0      893 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_bank_info_list.py
--rw-r--r--   0        0        0      888 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_benefit_list.py
--rw-r--r--   0        0        0      888 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_company_list.py
--rw-r--r--   0        0        0      921 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_condition_schema_list.py
--rw-r--r--   0        0        0      892 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_list.py
--rw-r--r--   0        0        0      934 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
--rw-r--r--   0        0        0      900 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employment_list.py
--rw-r--r--   0        0        0      880 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_group_list.py
--rw-r--r--   0        0        0      880 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_issue_list.py
--rw-r--r--   0        0        0      892 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_location_list.py
--rw-r--r--   0        0        0      893 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_pay_group_list.py
--rw-r--r--   0        0        0      901 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_payroll_run_list.py
--rw-r--r--   0        0        0      901 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_sync_status_list.py
--rw-r--r--   0        0        0      876 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_team_list.py
--rw-r--r--   0        0        0      918 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_balance_list.py
--rw-r--r--   0        0        0      889 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_list.py
--rw-r--r--   0        0        0    48882 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_currency_enum.py
--rw-r--r--   0        0        0     1940 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_frequency_enum.py
--rw-r--r--   0        0        0     1754 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_group.py
--rw-r--r--   0        0        0     1798 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/pay_period_enum.py
--rw-r--r--   0        0        0     2792 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run.py
--rw-r--r--   0        0        0      171 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run_run_type.py
--rw-r--r--   0        0        0      801 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
--rw-r--r--   0        0        0     1104 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
--rw-r--r--   0        0        0      813 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
--rw-r--r--   0        0        0      817 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0      829 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1305 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/policy_type_enum.py
--rw-r--r--   0        0        0      814 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/reason_enum.py
--rw-r--r--   0        0        0      802 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_data.py
--rw-r--r--   0        0        0      986 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_key.py
--rw-r--r--   0        0        0     1330 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_response.py
--rw-r--r--   0        0        0      195 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/remote_response_response_type.py
--rw-r--r--   0        0        0      723 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/request_format_enum.py
--rw-r--r--   0        0        0     1312 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/request_type_enum.py
--rw-r--r--   0        0        0      562 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/response_type_enum.py
--rw-r--r--   0        0        0     1032 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/run_state_enum.py
--rw-r--r--   0        0        0     1173 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/run_type_enum.py
--rw-r--r--   0        0        0      695 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
--rw-r--r--   0        0        0     1411 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/sync_status.py
--rw-r--r--   0        0        0     1333 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/sync_status_status_enum.py
--rw-r--r--   0        0        0     1975 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/tax.py
--rw-r--r--   0        0        0     1953 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/team.py
--rw-r--r--   0        0        0     3484 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off.py
--rw-r--r--   0        0        0     2517 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance.py
--rw-r--r--   0        0        0      187 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance_policy_type.py
--rw-r--r--   0        0        0     1272 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
--rw-r--r--   0        0        0      751 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_expand.py
--rw-r--r--   0        0        0     1595 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
--rw-r--r--   0        0        0     1223 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_request_type.py
--rw-r--r--   0        0        0     1619 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
--rw-r--r--   0        0        0     1029 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_status.py
--rw-r--r--   0        0        0     3158 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request.py
--rw-r--r--   0        0        0      191 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request_request_type.py
--rw-r--r--   0        0        0      184 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request_type.py
--rw-r--r--   0        0        0     1106 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_response.py
--rw-r--r--   0        0        0      767 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
--rw-r--r--   0        0        0     1627 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
--rw-r--r--   0        0        0     1651 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
--rw-r--r--   0        0        0     1146 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/time_off_status_enum.py
--rw-r--r--   0        0        0      495 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/units_enum.py
--rw-r--r--   0        0        0      762 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/validation_problem_source.py
--rw-r--r--   0        0        0      915 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/warning_validation_problem.py
--rw-r--r--   0        0        0      802 2023-07-12 19:36:44.488511 fern_merge-0.0.28/src/merge/resources/hris/types/webhook_receiver.py
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0     2139 2023-07-12 22:45:03.315861 fern_merge-0.0.29/README.md
+-rw-r--r--   0        0        0      371 2023-07-12 22:45:03.315861 fern_merge-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/client.py
+-rw-r--r--   0        0        0      528 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/api_error.py
+-rw-r--r--   0        0        0     1101 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      201 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/environment.py
+-rw-r--r--   0        0        0        0 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/py.typed
+-rw-r--r--   0        0        0      116 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/__init__.py
+-rw-r--r--   0        0        0     9656 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/__init__.py
+-rw-r--r--   0        0        0    10018 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/client.py
+-rw-r--r--   0        0        0     1144 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2284 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/activities/__init__.py
+-rw-r--r--   0        0        0    12088 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/activities/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/applications/__init__.py
+-rw-r--r--   0        0        0    14581 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/applications/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/attachments/__init__.py
+-rw-r--r--   0        0        0    11850 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/attachments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.315861 fern_merge-0.0.29/src/merge/resources/ats/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2304 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/candidates/__init__.py
+-rw-r--r--   0        0        0    16506 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/candidates/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2045 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/departments/__init__.py
+-rw-r--r--   0        0        0     5972 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/departments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/eeocs/__init__.py
+-rw-r--r--   0        0        0     8117 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/eeocs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2362 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/interviews/__init__.py
+-rw-r--r--   0        0        0    12540 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/interviews/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/issues/__init__.py
+-rw-r--r--   0        0        0     6768 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/job_interview_stages/__init__.py
+-rw-r--r--   0        0        0     6771 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/job_interview_stages/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     8227 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4774 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5305 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/offers/__init__.py
+-rw-r--r--   0        0        0     8095 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/offers/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/offices/__init__.py
+-rw-r--r--   0        0        0     5900 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/offices/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4816 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2545 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/reject_reasons/__init__.py
+-rw-r--r--   0        0        0     6014 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/reject_reasons/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/scorecards/__init__.py
+-rw-r--r--   0        0        0     8545 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/scorecards/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     6892 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2644 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/tags/__init__.py
+-rw-r--r--   0        0        0     4201 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/users/__init__.py
+-rw-r--r--   0        0        0     7399 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/users/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4191 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    13447 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/access_role_enum.py
+-rw-r--r--   0        0        0     1483 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/account_token.py
+-rw-r--r--   0        0        0      857 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activities_list_request_remote_fields.py
+-rw-r--r--   0        0        0      869 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      873 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      885 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     2705 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity.py
+-rw-r--r--   0        0        0      189 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_activity_type.py
+-rw-r--r--   0        0        0     2155 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_request.py
+-rw-r--r--   0        0        0      196 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_request_activity_type.py
+-rw-r--r--   0        0        0      187 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_request_visibility.py
+-rw-r--r--   0        0        0     1109 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_response.py
+-rw-r--r--   0        0        0      705 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_type_enum.py
+-rw-r--r--   0        0        0      180 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/activity_visibility.py
+-rw-r--r--   0        0        0     2473 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/application.py
+-rw-r--r--   0        0        0     2269 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/application_request.py
+-rw-r--r--   0        0        0     1121 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/application_response.py
+-rw-r--r--   0        0        0     8243 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/applications_list_request_expand.py
+-rw-r--r--   0        0        0     8371 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/applications_retrieve_request_expand.py
+-rw-r--r--   0        0        0     2146 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment.py
+-rw-r--r--   0        0        0      199 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment_attachment_type.py
+-rw-r--r--   0        0        0     1820 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment_request.py
+-rw-r--r--   0        0        0      206 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment_request_attachment_type.py
+-rw-r--r--   0        0        0     1117 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment_response.py
+-rw-r--r--   0        0        0      985 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/attachment_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/available_actions.py
+-rw-r--r--   0        0        0     3471 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/candidate.py
+-rw-r--r--   0        0        0     3061 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/candidate_request.py
+-rw-r--r--   0        0        0     1113 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/candidate_response.py
+-rw-r--r--   0        0        0      833 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/candidates_list_request_expand.py
+-rw-r--r--   0        0        0      849 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/candidates_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1391 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     2324 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/condition_type_enum.py
+-rw-r--r--   0        0        0      870 2023-07-12 22:45:03.319861 fern_merge-0.0.29/src/merge/resources/ats/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     1698 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/department.py
+-rw-r--r--   0        0        0     1337 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/disability_status_enum.py
+-rw-r--r--   0        0        0     4088 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeoc.py
+-rw-r--r--   0        0        0      201 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeoc_disability_status.py
+-rw-r--r--   0        0        0      160 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeoc_gender.py
+-rw-r--r--   0        0        0      152 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeoc_race.py
+-rw-r--r--   0        0        0      189 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeoc_veteran_status.py
+-rw-r--r--   0        0        0     3803 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     3851 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     3867 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     3915 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1529 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/email_address.py
+-rw-r--r--   0        0        0      210 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/email_address_email_address_type.py
+-rw-r--r--   0        0        0     1553 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/email_address_request.py
+-rw-r--r--   0        0        0      217 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/email_address_request_email_address_type.py
+-rw-r--r--   0        0        0      742 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/email_address_type_enum.py
+-rw-r--r--   0        0        0      522 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/error_validation_problem.py
+-rw-r--r--   0        0        0     1160 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/gender_enum.py
+-rw-r--r--   0        0        0     4187 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/interviews_list_request_expand.py
+-rw-r--r--   0        0        0     4251 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/interviews_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1323 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/issues_list_request_status.py
+-rw-r--r--   0        0        0     3428 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/job.py
+-rw-r--r--   0        0        0     2387 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/job_interview_stage.py
+-rw-r--r--   0        0        0      169 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/job_status.py
+-rw-r--r--   0        0        0     1045 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/job_status_enum.py
+-rw-r--r--   0        0        0     3771 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/jobs_list_request_expand.py
+-rw-r--r--   0        0        0      956 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/jobs_list_request_status.py
+-rw-r--r--   0        0        0     3835 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/jobs_retrieve_request_expand.py
+-rw-r--r--   0        0        0      835 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0     1037 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0     2786 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/offer.py
+-rw-r--r--   0        0        0      177 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/offer_status.py
+-rw-r--r--   0        0        0     1832 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/offer_status_enum.py
+-rw-r--r--   0        0        0      767 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/offers_list_request_expand.py
+-rw-r--r--   0        0        0      783 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/offers_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1817 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/office.py
+-rw-r--r--   0        0        0      993 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/operator_schema.py
+-rw-r--r--   0        0        0     1180 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/overall_recommendation_enum.py
+-rw-r--r--   0        0        0      959 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_activity_list.py
+-rw-r--r--   0        0        0      904 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_application_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_attachment_list.py
+-rw-r--r--   0        0        0      896 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_candidate_list.py
+-rw-r--r--   0        0        0      921 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_department_list.py
+-rw-r--r--   0        0        0      876 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_eeoc_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      930 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_job_interview_stage_list.py
+-rw-r--r--   0        0        0      872 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_job_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_offer_list.py
+-rw-r--r--   0        0        0      884 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_office_list.py
+-rw-r--r--   0        0        0      909 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_reject_reason_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_remote_user_list.py
+-rw-r--r--   0        0        0      933 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_scheduled_interview_list.py
+-rw-r--r--   0        0        0      896 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_scorecard_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      872 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/paginated_tag_list.py
+-rw-r--r--   0        0        0     3068 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/patched_candidate_request.py
+-rw-r--r--   0        0        0     1624 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/phone_number.py
+-rw-r--r--   0        0        0      205 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_phone_number_type.py
+-rw-r--r--   0        0        0     1648 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_request.py
+-rw-r--r--   0        0        0      212 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_request_phone_number_type.py
+-rw-r--r--   0        0        0     1039 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_type_enum.py
+-rw-r--r--   0        0        0     2326 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/race_enum.py
+-rw-r--r--   0        0        0      814 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/reason_enum.py
+-rw-r--r--   0        0        0     1775 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/reject_reason.py
+-rw-r--r--   0        0        0      802 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_response_response_type.py
+-rw-r--r--   0        0        0     2562 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_user.py
+-rw-r--r--   0        0        0      183 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/remote_user_access_role.py
+-rw-r--r--   0        0        0      723 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/request_format_enum.py
+-rw-r--r--   0        0        0      562 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/response_type_enum.py
+-rw-r--r--   0        0        0     3187 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview.py
+-rw-r--r--   0        0        0     2464 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_request.py
+-rw-r--r--   0        0        0      237 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_request_status.py
+-rw-r--r--   0        0        0     1150 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_response.py
+-rw-r--r--   0        0        0      230 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_status.py
+-rw-r--r--   0        0        0      893 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_status_enum.py
+-rw-r--r--   0        0        0     2692 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scorecard.py
+-rw-r--r--   0        0        0      226 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scorecard_overall_recommendation.py
+-rw-r--r--   0        0        0     1731 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scorecards_list_request_expand.py
+-rw-r--r--   0        0        0     1763 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py
+-rw-r--r--   0        0        0      695 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1623 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/tag.py
+-rw-r--r--   0        0        0     1659 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/url.py
+-rw-r--r--   0        0        0     1683 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/url_request.py
+-rw-r--r--   0        0        0      171 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/url_request_url_type.py
+-rw-r--r--   0        0        0     1451 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/url_type_enum.py
+-rw-r--r--   0        0        0      164 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/url_url_type.py
+-rw-r--r--   0        0        0      762 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/validation_problem_source.py
+-rw-r--r--   0        0        0     1467 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/veteran_status_enum.py
+-rw-r--r--   0        0        0      760 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/visibility_enum.py
+-rw-r--r--   0        0        0      915 2023-07-12 22:45:03.323861 fern_merge-0.0.29/src/merge/resources/ats/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/ats/types/webhook_receiver.py
+-rw-r--r--   0        0        0    10216 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/__init__.py
+-rw-r--r--   0        0        0     9511 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/client.py
+-rw-r--r--   0        0        0     1106 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/account_details/__init__.py
+-rw-r--r--   0        0        0     2286 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/account_details/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/account_token/__init__.py
+-rw-r--r--   0        0        0     2336 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/account_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/available_actions/__init__.py
+-rw-r--r--   0        0        0     2306 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/available_actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/bank_info/__init__.py
+-rw-r--r--   0        0        0     8705 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/bank_info/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/benefits/__init__.py
+-rw-r--r--   0        0        0     6633 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/benefits/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/companies/__init__.py
+-rw-r--r--   0        0        0     5928 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/companies/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/delete_account/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/delete_account/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employee_payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8024 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employee_payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employees/__init__.py
+-rw-r--r--   0        0        0    17328 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employees/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employments/__init__.py
+-rw-r--r--   0        0        0     8741 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/employments/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/force_resync/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/force_resync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/generate_key/__init__.py
+-rw-r--r--   0        0        0     2539 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/generate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/groups/__init__.py
+-rw-r--r--   0        0        0     7291 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/issues/__init__.py
+-rw-r--r--   0        0        0     6772 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/issues/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/link_token/__init__.py
+-rw-r--r--   0        0        0     4776 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/link_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/linked_accounts/__init__.py
+-rw-r--r--   0        0        0     5307 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/linked_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/locations/__init__.py
+-rw-r--r--   0        0        0     7265 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/locations/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/passthrough/__init__.py
+-rw-r--r--   0        0        0     4818 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/passthrough/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/pay_groups/__init__.py
+-rw-r--r--   0        0        0     5946 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/pay_groups/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/payroll_runs/__init__.py
+-rw-r--r--   0        0        0     8756 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/payroll_runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/regenerate_key/__init__.py
+-rw-r--r--   0        0        0     2547 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/regenerate_key/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/selective_sync/__init__.py
+-rw-r--r--   0        0        0     6898 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/selective_sync/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/sync_status/__init__.py
+-rw-r--r--   0        0        0     2646 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/sync_status/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/teams/__init__.py
+-rw-r--r--   0        0        0     6609 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/teams/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/time_off/__init__.py
+-rw-r--r--   0        0        0    12810 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/time_off/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/time_off_balances/__init__.py
+-rw-r--r--   0        0        0     8364 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/time_off_balances/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/webhook_receivers/__init__.py
+-rw-r--r--   0        0        0     4195 2023-07-12 22:45:03.327861 fern_merge-0.0.29/src/merge/resources/hris/resources/webhook_receivers/client.py
+-rw-r--r--   0        0        0    14432 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_details.py
+-rw-r--r--   0        0        0     1900 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions.py
+-rw-r--r--   0        0        0     1112 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions_integration.py
+-rw-r--r--   0        0        0      896 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions_status_enum.py
+-rw-r--r--   0        0        0     2342 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_integration.py
+-rw-r--r--   0        0        0      845 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_token.py
+-rw-r--r--   0        0        0      555 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/account_type_enum.py
+-rw-r--r--   0        0        0     1245 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/available_actions.py
+-rw-r--r--   0        0        0     2399 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/bank_info.py
+-rw-r--r--   0        0        0      185 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/bank_info_account_type.py
+-rw-r--r--   0        0        0      529 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/bank_info_list_request_account_type.py
+-rw-r--r--   0        0        0      728 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/bank_info_list_request_order_by.py
+-rw-r--r--   0        0        0     2342 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/benefit.py
+-rw-r--r--   0        0        0     1391 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/categories_enum.py
+-rw-r--r--   0        0        0     1375 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/category_enum.py
+-rw-r--r--   0        0        0      997 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/common_model_scopes_body_request.py
+-rw-r--r--   0        0        0     1962 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/company.py
+-rw-r--r--   0        0        0     2324 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/condition_schema.py
+-rw-r--r--   0        0        0      200 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/condition_schema_condition_type.py
+-rw-r--r--   0        0        0     1478 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/condition_type_enum.py
+-rw-r--r--   0        0        0    35178 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/country_enum.py
+-rw-r--r--   0        0        0      870 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/debug_mode_log.py
+-rw-r--r--   0        0        0      792 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/debug_model_log_summary.py
+-rw-r--r--   0        0        0     2140 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/deduction.py
+-rw-r--r--   0        0        0     2143 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/earning.py
+-rw-r--r--   0        0        0      177 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/earning_type.py
+-rw-r--r--   0        0        0      949 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/earning_type_enum.py
+-rw-r--r--   0        0        0     6788 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee.py
+-rw-r--r--   0        0        0      205 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_employment_status.py
+-rw-r--r--   0        0        0      176 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_ethnicity.py
+-rw-r--r--   0        0        0      164 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_gender.py
+-rw-r--r--   0        0        0      193 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_marital_status.py
+-rw-r--r--   0        0        0     2796 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_run.py
+-rw-r--r--   0        0        0      829 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py
+-rw-r--r--   0        0        0      845 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py
+-rw-r--r--   0        0        0     6252 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_request.py
+-rw-r--r--   0        0        0      212 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_request_employment_status.py
+-rw-r--r--   0        0        0      183 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_request_ethnicity.py
+-rw-r--r--   0        0        0      171 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_request_gender.py
+-rw-r--r--   0        0        0      200 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_request_marital_status.py
+-rw-r--r--   0        0        0     1109 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employee_response.py
+-rw-r--r--   0        0        0      739 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_employment_status.py
+-rw-r--r--   0        0        0    80247 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_expand.py
+-rw-r--r--   0        0        0     4067 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4115 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0    81343 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4131 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4179 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0    18682 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment.py
+-rw-r--r--   0        0        0      199 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_employment_type.py
+-rw-r--r--   0        0        0      183 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_flsa_status.py
+-rw-r--r--   0        0        0      187 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_pay_currency.py
+-rw-r--r--   0        0        0      191 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_pay_frequency.py
+-rw-r--r--   0        0        0      179 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_pay_period.py
+-rw-r--r--   0        0        0      770 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_status_enum.py
+-rw-r--r--   0        0        0     1166 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employment_type_enum.py
+-rw-r--r--   0        0        0      777 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_expand.py
+-rw-r--r--   0        0        0      707 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_order_by.py
+-rw-r--r--   0        0        0     4219 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_remote_fields.py
+-rw-r--r--   0        0        0     4267 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      793 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_expand.py
+-rw-r--r--   0        0        0     4283 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     4331 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      522 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/enabled_actions_enum.py
+-rw-r--r--   0        0        0      739 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/encoding_enum.py
+-rw-r--r--   0        0        0      913 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/error_validation_problem.py
+-rw-r--r--   0        0        0     2511 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/ethnicity_enum.py
+-rw-r--r--   0        0        0      986 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/flsa_status_enum.py
+-rw-r--r--   0        0        0     1146 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/gender_enum.py
+-rw-r--r--   0        0        0     2225 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/group.py
+-rw-r--r--   0        0        0      169 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/group_type.py
+-rw-r--r--   0        0        0     1136 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/group_type_enum.py
+-rw-r--r--   0        0        0     1323 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/issue.py
+-rw-r--r--   0        0        0      177 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/issue_status.py
+-rw-r--r--   0        0        0      555 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/issue_status_enum.py
+-rw-r--r--   0        0        0      508 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/issues_list_request_status.py
+-rw-r--r--   0        0        0      835 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/link_token.py
+-rw-r--r--   0        0        0     1488 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_condition.py
+-rw-r--r--   0        0        0     1079 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_condition_request.py
+-rw-r--r--   0        0        0      998 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py
+-rw-r--r--   0        0        0     1010 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py
+-rw-r--r--   0        0        0      799 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_status.py
+-rw-r--r--   0        0        0     1354 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/linked_accounts_list_request_category.py
+-rw-r--r--   0        0        0    11870 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/location.py
+-rw-r--r--   0        0        0      168 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/location_country.py
+-rw-r--r--   0        0        0      189 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/location_location_type.py
+-rw-r--r--   0        0        0      509 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/location_type_enum.py
+-rw-r--r--   0        0        0     1685 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/marital_status_enum.py
+-rw-r--r--   0        0        0     1037 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/meta_response.py
+-rw-r--r--   0        0        0     1275 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/method_enum.py
+-rw-r--r--   0        0        0     1162 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/model_operation.py
+-rw-r--r--   0        0        0     2012 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/multipart_form_field_request.py
+-rw-r--r--   0        0        0      189 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/multipart_form_field_request_encoding.py
+-rw-r--r--   0        0        0      993 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/operator_schema.py
+-rw-r--r--   0        0        0      959 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py
+-rw-r--r--   0        0        0      893 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_bank_info_list.py
+-rw-r--r--   0        0        0      888 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_benefit_list.py
+-rw-r--r--   0        0        0      888 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_company_list.py
+-rw-r--r--   0        0        0      921 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_condition_schema_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employee_list.py
+-rw-r--r--   0        0        0      934 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py
+-rw-r--r--   0        0        0      900 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employment_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_group_list.py
+-rw-r--r--   0        0        0      880 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_issue_list.py
+-rw-r--r--   0        0        0      892 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_location_list.py
+-rw-r--r--   0        0        0      893 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_pay_group_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_payroll_run_list.py
+-rw-r--r--   0        0        0      901 2023-07-12 22:45:03.331862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_sync_status_list.py
+-rw-r--r--   0        0        0      876 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_team_list.py
+-rw-r--r--   0        0        0      918 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_time_off_balance_list.py
+-rw-r--r--   0        0        0      889 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/paginated_time_off_list.py
+-rw-r--r--   0        0        0    48882 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/pay_currency_enum.py
+-rw-r--r--   0        0        0     1940 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/pay_frequency_enum.py
+-rw-r--r--   0        0        0     1754 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/pay_group.py
+-rw-r--r--   0        0        0     1798 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/pay_period_enum.py
+-rw-r--r--   0        0        0     2811 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_run.py
+-rw-r--r--   0        0        0      175 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_run_run_state.py
+-rw-r--r--   0        0        0      171 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_run_run_type.py
+-rw-r--r--   0        0        0      801 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1104 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py
+-rw-r--r--   0        0        0      813 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0      817 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0      829 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1305 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/policy_type_enum.py
+-rw-r--r--   0        0        0      814 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/reason_enum.py
+-rw-r--r--   0        0        0      802 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/remote_data.py
+-rw-r--r--   0        0        0      986 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/remote_key.py
+-rw-r--r--   0        0        0     1330 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/remote_response.py
+-rw-r--r--   0        0        0      195 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/remote_response_response_type.py
+-rw-r--r--   0        0        0      723 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/request_format_enum.py
+-rw-r--r--   0        0        0     1312 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/request_type_enum.py
+-rw-r--r--   0        0        0      562 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/response_type_enum.py
+-rw-r--r--   0        0        0     1032 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/run_state_enum.py
+-rw-r--r--   0        0        0     1173 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/run_type_enum.py
+-rw-r--r--   0        0        0      695 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py
+-rw-r--r--   0        0        0     1411 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/sync_status.py
+-rw-r--r--   0        0        0     1333 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/sync_status_status_enum.py
+-rw-r--r--   0        0        0     1975 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/tax.py
+-rw-r--r--   0        0        0     1953 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/team.py
+-rw-r--r--   0        0        0     3481 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off.py
+-rw-r--r--   0        0        0     2517 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_balance.py
+-rw-r--r--   0        0        0      187 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_balance_policy_type.py
+-rw-r--r--   0        0        0     1272 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py
+-rw-r--r--   0        0        0      751 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_expand.py
+-rw-r--r--   0        0        0     1595 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_remote_fields.py
+-rw-r--r--   0        0        0     1223 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_request_type.py
+-rw-r--r--   0        0        0     1619 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py
+-rw-r--r--   0        0        0     1029 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_status.py
+-rw-r--r--   0        0        0     3199 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request.py
+-rw-r--r--   0        0        0      191 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request_request_type.py
+-rw-r--r--   0        0        0      193 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request_status.py
+-rw-r--r--   0        0        0      184 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request_type.py
+-rw-r--r--   0        0        0      166 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request_units.py
+-rw-r--r--   0        0        0     1106 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_response.py
+-rw-r--r--   0        0        0      767 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_expand.py
+-rw-r--r--   0        0        0     1627 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py
+-rw-r--r--   0        0        0     1651 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py
+-rw-r--r--   0        0        0      186 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_status.py
+-rw-r--r--   0        0        0     1146 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_status_enum.py
+-rw-r--r--   0        0        0      159 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/time_off_units.py
+-rw-r--r--   0        0        0      495 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/units_enum.py
+-rw-r--r--   0        0        0      762 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/validation_problem_source.py
+-rw-r--r--   0        0        0      915 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/warning_validation_problem.py
+-rw-r--r--   0        0        0      802 2023-07-12 22:45:03.335862 fern_merge-0.0.29/src/merge/resources/hris/types/webhook_receiver.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 fern_merge-0.0.29/PKG-INFO
```

### Comparing `fern_merge-0.0.28/README.md` & `fern_merge-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/client.py` & `fern_merge-0.0.29/src/merge/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/core/__init__.py` & `fern_merge-0.0.29/src/merge/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/core/client_wrapper.py` & `fern_merge-0.0.29/src/merge/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/core/datetime_utils.py` & `fern_merge-0.0.29/src/merge/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/core/jsonable_encoder.py` & `fern_merge-0.0.29/src/merge/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/__init__.py` & `fern_merge-0.0.29/src/merge/resources/ats/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     ActivitiesListRequestShowEnumOrigins,
     ActivitiesRetrieveRequestRemoteFields,
     ActivitiesRetrieveRequestShowEnumOrigins,
     Activity,
     ActivityActivityType,
     ActivityRequest,
     ActivityRequestActivityType,
+    ActivityRequestVisibility,
     ActivityResponse,
     ActivityTypeEnum,
+    ActivityVisibility,
     Application,
     ApplicationRequest,
     ApplicationResponse,
     ApplicationsListRequestExpand,
     ApplicationsRetrieveRequestExpand,
     Attachment,
     AttachmentAttachmentType,
@@ -42,14 +44,18 @@
     ConditionSchemaConditionType,
     ConditionTypeEnum,
     DebugModeLog,
     DebugModelLogSummary,
     Department,
     DisabilityStatusEnum,
     Eeoc,
+    EeocDisabilityStatus,
+    EeocGender,
+    EeocRace,
+    EeocVeteranStatus,
     EeocsListRequestRemoteFields,
     EeocsListRequestShowEnumOrigins,
     EeocsRetrieveRequestRemoteFields,
     EeocsRetrieveRequestShowEnumOrigins,
     EmailAddress,
     EmailAddressEmailAddressType,
     EmailAddressRequest,
@@ -58,18 +64,20 @@
     EnabledActionsEnum,
     EncodingEnum,
     ErrorValidationProblem,
     GenderEnum,
     InterviewsListRequestExpand,
     InterviewsRetrieveRequestExpand,
     Issue,
+    IssueStatus,
     IssueStatusEnum,
     IssuesListRequestStatus,
     Job,
     JobInterviewStage,
+    JobStatus,
     JobStatusEnum,
     JobsListRequestExpand,
     JobsListRequestStatus,
     JobsRetrieveRequestExpand,
     LinkToken,
     LinkedAccountCondition,
     LinkedAccountConditionRequest,
@@ -77,15 +85,17 @@
     LinkedAccountSelectiveSyncConfigurationRequest,
     LinkedAccountStatus,
     LinkedAccountsListRequestCategory,
     MetaResponse,
     MethodEnum,
     ModelOperation,
     MultipartFormFieldRequest,
+    MultipartFormFieldRequestEncoding,
     Offer,
+    OfferStatus,
     OfferStatusEnum,
     OffersListRequestExpand,
     OffersRetrieveRequestExpand,
     Office,
     OperatorSchema,
     OverallRecommendationEnum,
     PaginatedAccountDetailsAndActionsList,
@@ -117,21 +127,25 @@
     ReasonEnum,
     RejectReason,
     RemoteData,
     RemoteKey,
     RemoteResponse,
     RemoteResponseResponseType,
     RemoteUser,
+    RemoteUserAccessRole,
     RequestFormatEnum,
     ResponseTypeEnum,
     ScheduledInterview,
     ScheduledInterviewRequest,
+    ScheduledInterviewRequestStatus,
     ScheduledInterviewResponse,
+    ScheduledInterviewStatus,
     ScheduledInterviewStatusEnum,
     Scorecard,
+    ScorecardOverallRecommendation,
     ScorecardsListRequestExpand,
     ScorecardsRetrieveRequestExpand,
     SelectiveSyncConfigurationsUsageEnum,
     SyncStatus,
     SyncStatusStatusEnum,
     Tag,
     Url,
@@ -189,16 +203,18 @@
     "ActivitiesListRequestShowEnumOrigins",
     "ActivitiesRetrieveRequestRemoteFields",
     "ActivitiesRetrieveRequestShowEnumOrigins",
     "Activity",
     "ActivityActivityType",
     "ActivityRequest",
     "ActivityRequestActivityType",
+    "ActivityRequestVisibility",
     "ActivityResponse",
     "ActivityTypeEnum",
+    "ActivityVisibility",
     "Application",
     "ApplicationRequest",
     "ApplicationResponse",
     "ApplicationsListRequestExpand",
     "ApplicationsRetrieveRequestExpand",
     "Attachment",
     "AttachmentAttachmentType",
@@ -219,14 +235,18 @@
     "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Department",
     "DisabilityStatusEnum",
     "Eeoc",
+    "EeocDisabilityStatus",
+    "EeocGender",
+    "EeocRace",
+    "EeocVeteranStatus",
     "EeocsListRequestRemoteFields",
     "EeocsListRequestShowEnumOrigins",
     "EeocsRetrieveRequestRemoteFields",
     "EeocsRetrieveRequestShowEnumOrigins",
     "EmailAddress",
     "EmailAddressEmailAddressType",
     "EmailAddressRequest",
@@ -235,18 +255,20 @@
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "GenderEnum",
     "InterviewsListRequestExpand",
     "InterviewsRetrieveRequestExpand",
     "Issue",
+    "IssueStatus",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "Job",
     "JobInterviewStage",
+    "JobStatus",
     "JobStatusEnum",
     "JobsListRequestExpand",
     "JobsListRequestStatus",
     "JobsRetrieveRequestExpand",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
@@ -254,15 +276,17 @@
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
+    "MultipartFormFieldRequestEncoding",
     "Offer",
+    "OfferStatus",
     "OfferStatusEnum",
     "OffersListRequestExpand",
     "OffersRetrieveRequestExpand",
     "Office",
     "OperatorSchema",
     "OverallRecommendationEnum",
     "PaginatedAccountDetailsAndActionsList",
@@ -294,21 +318,25 @@
     "ReasonEnum",
     "RejectReason",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
     "RemoteResponseResponseType",
     "RemoteUser",
+    "RemoteUserAccessRole",
     "RequestFormatEnum",
     "ResponseTypeEnum",
     "ScheduledInterview",
     "ScheduledInterviewRequest",
+    "ScheduledInterviewRequestStatus",
     "ScheduledInterviewResponse",
+    "ScheduledInterviewStatus",
     "ScheduledInterviewStatusEnum",
     "Scorecard",
+    "ScorecardOverallRecommendation",
     "ScorecardsListRequestExpand",
     "ScorecardsRetrieveRequestExpand",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tag",
     "Url",
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/__init__.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/account_details/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/account_token/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/activities/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/activities/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/applications/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/applications/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/attachments/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/attachments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/available_actions/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/candidates/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/candidates/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/delete_account/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/departments/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/departments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/eeocs/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/eeocs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/force_resync/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/generate_key/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/interviews/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/interviews/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/issues/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/job_interview_stages/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/job_interview_stages/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/jobs/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/link_token/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/linked_accounts/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/offers/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/offers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/offices/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/offices/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/passthrough/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/regenerate_key/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/reject_reasons/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/reject_reasons/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/scorecards/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/scorecards/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/selective_sync/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/sync_status/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/tags/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/users/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/resources/webhook_receivers/client.py` & `fern_merge-0.0.29/src/merge/resources/ats/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/__init__.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 from .activities_list_request_show_enum_origins import ActivitiesListRequestShowEnumOrigins
 from .activities_retrieve_request_remote_fields import ActivitiesRetrieveRequestRemoteFields
 from .activities_retrieve_request_show_enum_origins import ActivitiesRetrieveRequestShowEnumOrigins
 from .activity import Activity
 from .activity_activity_type import ActivityActivityType
 from .activity_request import ActivityRequest
 from .activity_request_activity_type import ActivityRequestActivityType
+from .activity_request_visibility import ActivityRequestVisibility
 from .activity_response import ActivityResponse
 from .activity_type_enum import ActivityTypeEnum
+from .activity_visibility import ActivityVisibility
 from .application import Application
 from .application_request import ApplicationRequest
 from .application_response import ApplicationResponse
 from .applications_list_request_expand import ApplicationsListRequestExpand
 from .applications_retrieve_request_expand import ApplicationsRetrieveRequestExpand
 from .attachment import Attachment
 from .attachment_attachment_type import AttachmentAttachmentType
@@ -41,14 +43,18 @@
 from .condition_schema_condition_type import ConditionSchemaConditionType
 from .condition_type_enum import ConditionTypeEnum
 from .debug_mode_log import DebugModeLog
 from .debug_model_log_summary import DebugModelLogSummary
 from .department import Department
 from .disability_status_enum import DisabilityStatusEnum
 from .eeoc import Eeoc
+from .eeoc_disability_status import EeocDisabilityStatus
+from .eeoc_gender import EeocGender
+from .eeoc_race import EeocRace
+from .eeoc_veteran_status import EeocVeteranStatus
 from .eeocs_list_request_remote_fields import EeocsListRequestRemoteFields
 from .eeocs_list_request_show_enum_origins import EeocsListRequestShowEnumOrigins
 from .eeocs_retrieve_request_remote_fields import EeocsRetrieveRequestRemoteFields
 from .eeocs_retrieve_request_show_enum_origins import EeocsRetrieveRequestShowEnumOrigins
 from .email_address import EmailAddress
 from .email_address_email_address_type import EmailAddressEmailAddressType
 from .email_address_request import EmailAddressRequest
@@ -57,18 +63,20 @@
 from .enabled_actions_enum import EnabledActionsEnum
 from .encoding_enum import EncodingEnum
 from .error_validation_problem import ErrorValidationProblem
 from .gender_enum import GenderEnum
 from .interviews_list_request_expand import InterviewsListRequestExpand
 from .interviews_retrieve_request_expand import InterviewsRetrieveRequestExpand
 from .issue import Issue
+from .issue_status import IssueStatus
 from .issue_status_enum import IssueStatusEnum
 from .issues_list_request_status import IssuesListRequestStatus
 from .job import Job
 from .job_interview_stage import JobInterviewStage
+from .job_status import JobStatus
 from .job_status_enum import JobStatusEnum
 from .jobs_list_request_expand import JobsListRequestExpand
 from .jobs_list_request_status import JobsListRequestStatus
 from .jobs_retrieve_request_expand import JobsRetrieveRequestExpand
 from .link_token import LinkToken
 from .linked_account_condition import LinkedAccountCondition
 from .linked_account_condition_request import LinkedAccountConditionRequest
@@ -76,15 +84,17 @@
 from .linked_account_selective_sync_configuration_request import LinkedAccountSelectiveSyncConfigurationRequest
 from .linked_account_status import LinkedAccountStatus
 from .linked_accounts_list_request_category import LinkedAccountsListRequestCategory
 from .meta_response import MetaResponse
 from .method_enum import MethodEnum
 from .model_operation import ModelOperation
 from .multipart_form_field_request import MultipartFormFieldRequest
+from .multipart_form_field_request_encoding import MultipartFormFieldRequestEncoding
 from .offer import Offer
+from .offer_status import OfferStatus
 from .offer_status_enum import OfferStatusEnum
 from .offers_list_request_expand import OffersListRequestExpand
 from .offers_retrieve_request_expand import OffersRetrieveRequestExpand
 from .office import Office
 from .operator_schema import OperatorSchema
 from .overall_recommendation_enum import OverallRecommendationEnum
 from .paginated_account_details_and_actions_list import PaginatedAccountDetailsAndActionsList
@@ -116,21 +126,25 @@
 from .reason_enum import ReasonEnum
 from .reject_reason import RejectReason
 from .remote_data import RemoteData
 from .remote_key import RemoteKey
 from .remote_response import RemoteResponse
 from .remote_response_response_type import RemoteResponseResponseType
 from .remote_user import RemoteUser
+from .remote_user_access_role import RemoteUserAccessRole
 from .request_format_enum import RequestFormatEnum
 from .response_type_enum import ResponseTypeEnum
 from .scheduled_interview import ScheduledInterview
 from .scheduled_interview_request import ScheduledInterviewRequest
+from .scheduled_interview_request_status import ScheduledInterviewRequestStatus
 from .scheduled_interview_response import ScheduledInterviewResponse
+from .scheduled_interview_status import ScheduledInterviewStatus
 from .scheduled_interview_status_enum import ScheduledInterviewStatusEnum
 from .scorecard import Scorecard
+from .scorecard_overall_recommendation import ScorecardOverallRecommendation
 from .scorecards_list_request_expand import ScorecardsListRequestExpand
 from .scorecards_retrieve_request_expand import ScorecardsRetrieveRequestExpand
 from .selective_sync_configurations_usage_enum import SelectiveSyncConfigurationsUsageEnum
 from .sync_status import SyncStatus
 from .sync_status_status_enum import SyncStatusStatusEnum
 from .tag import Tag
 from .url import Url
@@ -156,16 +170,18 @@
     "ActivitiesListRequestShowEnumOrigins",
     "ActivitiesRetrieveRequestRemoteFields",
     "ActivitiesRetrieveRequestShowEnumOrigins",
     "Activity",
     "ActivityActivityType",
     "ActivityRequest",
     "ActivityRequestActivityType",
+    "ActivityRequestVisibility",
     "ActivityResponse",
     "ActivityTypeEnum",
+    "ActivityVisibility",
     "Application",
     "ApplicationRequest",
     "ApplicationResponse",
     "ApplicationsListRequestExpand",
     "ApplicationsRetrieveRequestExpand",
     "Attachment",
     "AttachmentAttachmentType",
@@ -186,14 +202,18 @@
     "ConditionSchemaConditionType",
     "ConditionTypeEnum",
     "DebugModeLog",
     "DebugModelLogSummary",
     "Department",
     "DisabilityStatusEnum",
     "Eeoc",
+    "EeocDisabilityStatus",
+    "EeocGender",
+    "EeocRace",
+    "EeocVeteranStatus",
     "EeocsListRequestRemoteFields",
     "EeocsListRequestShowEnumOrigins",
     "EeocsRetrieveRequestRemoteFields",
     "EeocsRetrieveRequestShowEnumOrigins",
     "EmailAddress",
     "EmailAddressEmailAddressType",
     "EmailAddressRequest",
@@ -202,18 +222,20 @@
     "EnabledActionsEnum",
     "EncodingEnum",
     "ErrorValidationProblem",
     "GenderEnum",
     "InterviewsListRequestExpand",
     "InterviewsRetrieveRequestExpand",
     "Issue",
+    "IssueStatus",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "Job",
     "JobInterviewStage",
+    "JobStatus",
     "JobStatusEnum",
     "JobsListRequestExpand",
     "JobsListRequestStatus",
     "JobsRetrieveRequestExpand",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
@@ -221,15 +243,17 @@
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
+    "MultipartFormFieldRequestEncoding",
     "Offer",
+    "OfferStatus",
     "OfferStatusEnum",
     "OffersListRequestExpand",
     "OffersRetrieveRequestExpand",
     "Office",
     "OperatorSchema",
     "OverallRecommendationEnum",
     "PaginatedAccountDetailsAndActionsList",
@@ -261,21 +285,25 @@
     "ReasonEnum",
     "RejectReason",
     "RemoteData",
     "RemoteKey",
     "RemoteResponse",
     "RemoteResponseResponseType",
     "RemoteUser",
+    "RemoteUserAccessRole",
     "RequestFormatEnum",
     "ResponseTypeEnum",
     "ScheduledInterview",
     "ScheduledInterviewRequest",
+    "ScheduledInterviewRequestStatus",
     "ScheduledInterviewResponse",
+    "ScheduledInterviewStatus",
     "ScheduledInterviewStatusEnum",
     "Scorecard",
+    "ScorecardOverallRecommendation",
     "ScorecardsListRequestExpand",
     "ScorecardsRetrieveRequestExpand",
     "SelectiveSyncConfigurationsUsageEnum",
     "SyncStatus",
     "SyncStatusStatusEnum",
     "Tag",
     "Url",
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/access_role_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/access_role_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_details.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_integration.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_integration.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/account_token.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activities_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activities_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activities_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activities_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activity.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .activity_activity_type import ActivityActivityType
+from .activity_visibility import ActivityVisibility
 from .remote_data import RemoteData
-from .visibility_enum import VisibilityEnum
 
 
 class Activity(pydantic.BaseModel):
     """
     # The Activity Object
     ### Description
     The `Activity` object is used to represent an activity for a candidate performed by a user.
@@ -25,15 +25,15 @@
     user: typing.Optional[str] = pydantic.Field(description="The user that performed the action.")
     remote_created_at: typing.Optional[str] = pydantic.Field(description="When the third party's activity was created.")
     activity_type: typing.Optional[ActivityActivityType] = pydantic.Field(
         description=("The activity's type.\n" "\n" "* `NOTE` - NOTE\n" "* `EMAIL` - EMAIL\n" "* `OTHER` - OTHER\n")
     )
     subject: typing.Optional[str] = pydantic.Field(description="The activity's subject.")
     body: typing.Optional[str] = pydantic.Field(description="The activity's body.")
-    visibility: typing.Optional[VisibilityEnum] = pydantic.Field(
+    visibility: typing.Optional[ActivityVisibility] = pydantic.Field(
         description=(
             "The activity's visibility.\n"
             "\n"
             "* `ADMIN_ONLY` - ADMIN_ONLY\n"
             "* `PUBLIC` - PUBLIC\n"
             "* `PRIVATE` - PRIVATE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activity_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activity_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .activity_request_activity_type import ActivityRequestActivityType
-from .visibility_enum import VisibilityEnum
+from .activity_request_visibility import ActivityRequestVisibility
 
 
 class ActivityRequest(pydantic.BaseModel):
     """
     # The Activity Object
     ### Description
     The `Activity` object is used to represent an activity for a candidate performed by a user.
@@ -21,15 +21,15 @@
 
     user: typing.Optional[str] = pydantic.Field(description="The user that performed the action.")
     activity_type: typing.Optional[ActivityRequestActivityType] = pydantic.Field(
         description=("The activity's type.\n" "\n" "* `NOTE` - NOTE\n" "* `EMAIL` - EMAIL\n" "* `OTHER` - OTHER\n")
     )
     subject: typing.Optional[str] = pydantic.Field(description="The activity's subject.")
     body: typing.Optional[str] = pydantic.Field(description="The activity's body.")
-    visibility: typing.Optional[VisibilityEnum] = pydantic.Field(
+    visibility: typing.Optional[ActivityRequestVisibility] = pydantic.Field(
         description=(
             "The activity's visibility.\n"
             "\n"
             "* `ADMIN_ONLY` - ADMIN_ONLY\n"
             "* `PUBLIC` - PUBLIC\n"
             "* `PRIVATE` - PRIVATE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activity_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activity_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/activity_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/activity_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/application.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/application.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/application_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/application_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/application_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/application_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/applications_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/applications_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/applications_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/applications_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/attachment.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/attachment.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/attachment_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/attachment_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/attachment_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/attachment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/available_actions.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/candidate.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/candidate.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/candidate_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/candidate_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/candidate_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/candidates_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/candidates_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/candidates_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/candidates_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/categories_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/category_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/common_model_scopes_body_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/condition_schema.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/condition_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/debug_mode_log.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/debug_model_log_summary.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/department.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/department.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/disability_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/disability_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/eeoc.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/eeoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .disability_status_enum import DisabilityStatusEnum
-from .gender_enum import GenderEnum
-from .race_enum import RaceEnum
+from .eeoc_disability_status import EeocDisabilityStatus
+from .eeoc_gender import EeocGender
+from .eeoc_race import EeocRace
+from .eeoc_veteran_status import EeocVeteranStatus
 from .remote_data import RemoteData
-from .veteran_status_enum import VeteranStatusEnum
 
 
 class Eeoc(pydantic.BaseModel):
     """
     # The EEOC Object
     ### Description
     The `EEOC` object is used to represent the Equal Employment Opportunity Commission information for a candidate (race, gender, veteran status, disability status).
@@ -22,49 +22,49 @@
     Fetch from the `LIST EEOCs` endpoint and filter by `candidate` to show all EEOC information for a candidate.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     candidate: typing.Optional[str] = pydantic.Field(description="The candidate being represented.")
     submitted_at: typing.Optional[str] = pydantic.Field(description="When the information was submitted.")
-    race: typing.Optional[RaceEnum] = pydantic.Field(
+    race: typing.Optional[EeocRace] = pydantic.Field(
         description=(
             "The candidate's race.\n"
             "\n"
             "* `AMERICAN_INDIAN_OR_ALASKAN_NATIVE` - AMERICAN_INDIAN_OR_ALASKAN_NATIVE\n"
             "* `ASIAN` - ASIAN\n"
             "* `BLACK_OR_AFRICAN_AMERICAN` - BLACK_OR_AFRICAN_AMERICAN\n"
             "* `HISPANIC_OR_LATINO` - HISPANIC_OR_LATINO\n"
             "* `WHITE` - WHITE\n"
             "* `NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER` - NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER\n"
             "* `TWO_OR_MORE_RACES` - TWO_OR_MORE_RACES\n"
             "* `DECLINE_TO_SELF_IDENTIFY` - DECLINE_TO_SELF_IDENTIFY\n"
         )
     )
-    gender: typing.Optional[GenderEnum] = pydantic.Field(
+    gender: typing.Optional[EeocGender] = pydantic.Field(
         description=(
             "The candidate's gender.\n"
             "\n"
             "* `MALE` - MALE\n"
             "* `FEMALE` - FEMALE\n"
             "* `NON-BINARY` - NON-BINARY\n"
             "* `OTHER` - OTHER\n"
             "* `DECLINE_TO_SELF_IDENTIFY` - DECLINE_TO_SELF_IDENTIFY\n"
         )
     )
-    veteran_status: typing.Optional[VeteranStatusEnum] = pydantic.Field(
+    veteran_status: typing.Optional[EeocVeteranStatus] = pydantic.Field(
         description=(
             "The candidate's veteran status.\n"
             "\n"
             "* `I_AM_NOT_A_PROTECTED_VETERAN` - I_AM_NOT_A_PROTECTED_VETERAN\n"
             "* `I_IDENTIFY_AS_ONE_OR_MORE_OF_THE_CLASSIFICATIONS_OF_A_PROTECTED_VETERAN` - I_IDENTIFY_AS_ONE_OR_MORE_OF_THE_CLASSIFICATIONS_OF_A_PROTECTED_VETERAN\n"
             "* `I_DONT_WISH_TO_ANSWER` - I_DONT_WISH_TO_ANSWER\n"
         )
     )
-    disability_status: typing.Optional[DisabilityStatusEnum] = pydantic.Field(
+    disability_status: typing.Optional[EeocDisabilityStatus] = pydantic.Field(
         description=(
             "The candidate's disability status.\n"
             "\n"
             "* `YES_I_HAVE_A_DISABILITY_OR_PREVIOUSLY_HAD_A_DISABILITY` - YES_I_HAVE_A_DISABILITY_OR_PREVIOUSLY_HAD_A_DISABILITY\n"
             "* `NO_I_DONT_HAVE_A_DISABILITY` - NO_I_DONT_HAVE_A_DISABILITY\n"
             "* `I_DONT_WISH_TO_ANSWER` - I_DONT_WISH_TO_ANSWER\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/eeocs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/email_address.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/email_address.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/email_address_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/email_address_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/email_address_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/email_address_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/enabled_actions_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/encoding_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/error_validation_problem.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/gender_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/interviews_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/interviews_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/interviews_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/interviews_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/issue.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .issue_status_enum import IssueStatusEnum
+from .issue_status import IssueStatus
 
 
 class Issue(pydantic.BaseModel):
     id: typing.Optional[str]
-    status: typing.Optional[IssueStatusEnum] = pydantic.Field(
+    status: typing.Optional[IssueStatus] = pydantic.Field(
         description=(
             "Status of the issue. Options: ('ONGOING', 'RESOLVED')\n"
             "\n"
             "* `ONGOING` - ONGOING\n"
             "* `RESOLVED` - RESOLVED\n"
         )
     )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/issue_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/job.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .job_status_enum import JobStatusEnum
+from .job_status import JobStatus
 from .remote_data import RemoteData
 from .url import Url
 
 
 class Job(pydantic.BaseModel):
     """
     # The Job Object
@@ -23,15 +23,15 @@
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     name: typing.Optional[str] = pydantic.Field(description="The job's name.")
     description: typing.Optional[str] = pydantic.Field(description="The job's description.")
     code: typing.Optional[str] = pydantic.Field(
         description="The job's code. Typically an additional identifier used to reference the particular job that is displayed on the ATS."
     )
-    status: typing.Optional[JobStatusEnum] = pydantic.Field(
+    status: typing.Optional[JobStatus] = pydantic.Field(
         description=(
             "The job's status.\n"
             "\n"
             "* `OPEN` - OPEN\n"
             "* `CLOSED` - CLOSED\n"
             "* `DRAFT` - DRAFT\n"
             "* `ARCHIVED` - ARCHIVED\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/job_interview_stage.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/job_interview_stage.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/job_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/job_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/jobs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_list_request_status.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/jobs_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/jobs_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/jobs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/link_token.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_condition_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_account_status.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/meta_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/method_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/model_operation.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/multipart_form_field_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/multipart_form_field_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .encoding_enum import EncodingEnum
+from .multipart_form_field_request_encoding import MultipartFormFieldRequestEncoding
 
 
 class MultipartFormFieldRequest(pydantic.BaseModel):
     """
     # The MultipartFormField Object
     ### Description
     The `MultipartFormField` object is used to represent fields in an HTTP request using `multipart/form-data`.
@@ -21,15 +21,15 @@
 
     name: str = pydantic.Field(
         description='The name of the form field <span style="white-space: nowrap">`non-empty`</span> '
     )
     data: str = pydantic.Field(
         description='The data for the form field. <span style="white-space: nowrap">`non-empty`</span> '
     )
-    encoding: typing.Optional[EncodingEnum] = pydantic.Field(
+    encoding: typing.Optional[MultipartFormFieldRequestEncoding] = pydantic.Field(
         description=(
             "The encoding of the value of `data`. Defaults to `RAW` if not defined.\n"
             "\n"
             "* `RAW` - RAW\n"
             "* `BASE64` - BASE64\n"
             "* `GZIP_BASE64` - GZIP_BASE64\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/offer.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/offer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .offer_status_enum import OfferStatusEnum
+from .offer_status import OfferStatus
 from .remote_data import RemoteData
 
 
 class Offer(pydantic.BaseModel):
     """
     # The Offer Object
     ### Description
@@ -23,15 +23,15 @@
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     application: typing.Optional[str] = pydantic.Field(description="The application who is receiving the offer.")
     creator: typing.Optional[str] = pydantic.Field(description="The user who created the offer.")
     remote_created_at: typing.Optional[str] = pydantic.Field(description="When the third party's offer was created.")
     closed_at: typing.Optional[str] = pydantic.Field(description="When the offer was closed.")
     sent_at: typing.Optional[str] = pydantic.Field(description="When the offer was sent.")
     start_date: typing.Optional[str] = pydantic.Field(description="The employment start date on the offer.")
-    status: typing.Optional[OfferStatusEnum] = pydantic.Field(
+    status: typing.Optional[OfferStatus] = pydantic.Field(
         description=(
             "The offer's status.\n"
             "\n"
             "* `DRAFT` - DRAFT\n"
             "* `APPROVAL-SENT` - APPROVAL-SENT\n"
             "* `APPROVED` - APPROVED\n"
             "* `SENT` - SENT\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/offer_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/offer_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/offers_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/offers_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/offers_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/offers_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/office.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/office.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/operator_schema.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/overall_recommendation_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/overall_recommendation_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_activity_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_activity_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_application_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_application_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_attachment_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_candidate_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_candidate_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_condition_schema_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_department_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_department_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_eeoc_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_eeoc_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_issue_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_interview_stage_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_job_interview_stage_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_job_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_job_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_offer_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_offer_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_office_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_office_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_reject_reason_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_reject_reason_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_remote_user_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_remote_user_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scheduled_interview_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_scheduled_interview_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_scorecard_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_scorecard_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_sync_status_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/paginated_tag_list.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/paginated_tag_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/patched_candidate_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/patched_candidate_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/phone_number.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/phone_number_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/phone_number_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/race_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/race_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/reason_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/reject_reason.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/reject_reason.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/remote_data.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/remote_key.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/remote_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/remote_user.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/remote_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .access_role_enum import AccessRoleEnum
 from .remote_data import RemoteData
+from .remote_user_access_role import RemoteUserAccessRole
 
 
 class RemoteUser(pydantic.BaseModel):
     """
     # The RemoteUser Object
     ### Description
     The `RemoteUser` object is used to represent a user with a login to the ATS system.
@@ -22,15 +22,15 @@
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     first_name: typing.Optional[str] = pydantic.Field(description="The user's first name.")
     last_name: typing.Optional[str] = pydantic.Field(description="The user's last name.")
     email: typing.Optional[str] = pydantic.Field(description="The user's email.")
     disabled: typing.Optional[bool] = pydantic.Field(description="Whether the user's account had been disabled.")
     remote_created_at: typing.Optional[str] = pydantic.Field(description="When the third party's user was created.")
-    access_role: typing.Optional[AccessRoleEnum] = pydantic.Field(
+    access_role: typing.Optional[RemoteUserAccessRole] = pydantic.Field(
         description=(
             "The user's role.\n"
             "\n"
             "* `SUPER_ADMIN` - SUPER_ADMIN\n"
             "* `ADMIN` - ADMIN\n"
             "* `TEAM_MEMBER` - TEAM_MEMBER\n"
             "* `LIMITED_TEAM_MEMBER` - LIMITED_TEAM_MEMBER\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/request_format_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/response_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .remote_data import RemoteData
-from .scheduled_interview_status_enum import ScheduledInterviewStatusEnum
+from .scheduled_interview_status import ScheduledInterviewStatus
 
 
 class ScheduledInterview(pydantic.BaseModel):
     """
     # The ScheduledInterview Object
     ### Description
     The `ScheduledInterview` object is used to represent a scheduled interview for a given candidate’s application to a job. An `Application` can have multiple `ScheduledInterview`s depending on the particular hiring process.
@@ -32,15 +32,15 @@
     end_at: typing.Optional[str] = pydantic.Field(description="When the interview was ended.")
     remote_created_at: typing.Optional[str] = pydantic.Field(
         description="When the third party's interview was created."
     )
     remote_updated_at: typing.Optional[str] = pydantic.Field(
         description="When the third party's interview was updated."
     )
-    status: typing.Optional[ScheduledInterviewStatusEnum] = pydantic.Field(
+    status: typing.Optional[ScheduledInterviewStatus] = pydantic.Field(
         description=(
             "The interview's status.\n"
             "\n"
             "* `SCHEDULED` - SCHEDULED\n"
             "* `AWAITING_FEEDBACK` - AWAITING_FEEDBACK\n"
             "* `COMPLETE` - COMPLETE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .scheduled_interview_status_enum import ScheduledInterviewStatusEnum
+from .scheduled_interview_request_status import ScheduledInterviewRequestStatus
 
 
 class ScheduledInterviewRequest(pydantic.BaseModel):
     """
     # The ScheduledInterview Object
     ### Description
     The `ScheduledInterview` object is used to represent a scheduled interview for a given candidate’s application to a job. An `Application` can have multiple `ScheduledInterview`s depending on the particular hiring process.
@@ -23,15 +23,15 @@
     organizer: typing.Optional[str] = pydantic.Field(description="The user organizing the interview.")
     interviewers: typing.Optional[typing.List[typing.Optional[str]]] = pydantic.Field(
         description="Array of `RemoteUser` IDs."
     )
     location: typing.Optional[str] = pydantic.Field(description="The interview's location.")
     start_at: typing.Optional[str] = pydantic.Field(description="When the interview was started.")
     end_at: typing.Optional[str] = pydantic.Field(description="When the interview was ended.")
-    status: typing.Optional[ScheduledInterviewStatusEnum] = pydantic.Field(
+    status: typing.Optional[ScheduledInterviewRequestStatus] = pydantic.Field(
         description=(
             "The interview's status.\n"
             "\n"
             "* `SCHEDULED` - SCHEDULED\n"
             "* `AWAITING_FEEDBACK` - AWAITING_FEEDBACK\n"
             "* `COMPLETE` - COMPLETE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_response.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scheduled_interview_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scheduled_interview_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scorecard.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scorecard.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .overall_recommendation_enum import OverallRecommendationEnum
 from .remote_data import RemoteData
+from .scorecard_overall_recommendation import ScorecardOverallRecommendation
 
 
 class Scorecard(pydantic.BaseModel):
     """
     # The Scorecard Object
     ### Description
     The `Scorecard` object is used to represent an interviewer's candidate recommendation based on a particular interview.
@@ -24,15 +24,15 @@
     application: typing.Optional[str] = pydantic.Field(description="The application being scored.")
     interview: typing.Optional[str] = pydantic.Field(description="The interview being scored.")
     interviewer: typing.Optional[str] = pydantic.Field(description="The interviewer doing the scoring.")
     remote_created_at: typing.Optional[str] = pydantic.Field(
         description="When the third party's scorecard was created."
     )
     submitted_at: typing.Optional[str] = pydantic.Field(description="When the scorecard was submitted.")
-    overall_recommendation: typing.Optional[OverallRecommendationEnum] = pydantic.Field(
+    overall_recommendation: typing.Optional[ScorecardOverallRecommendation] = pydantic.Field(
         description=(
             "The inteviewer's recommendation.\n"
             "\n"
             "* `DEFINITELY_NO` - DEFINITELY_NO\n"
             "* `NO` - NO\n"
             "* `YES` - YES\n"
             "* `STRONG_YES` - STRONG_YES\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scorecards_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/scorecards_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/sync_status.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/sync_status_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/tag.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/tag.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/url.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/url.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/url_request.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/url_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/url_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/url_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/validation_problem_source.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/veteran_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/veteran_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/visibility_enum.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/visibility_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/warning_validation_problem.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/ats/types/webhook_receiver.py` & `fern_merge-0.0.29/src/merge/resources/ats/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/__init__.py` & `fern_merge-0.0.29/src/merge/resources/hris/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,28 +25,40 @@
     DebugModeLog,
     DebugModelLogSummary,
     Deduction,
     Earning,
     EarningType,
     EarningTypeEnum,
     Employee,
+    EmployeeEmploymentStatus,
+    EmployeeEthnicity,
+    EmployeeGender,
+    EmployeeMaritalStatus,
     EmployeePayrollRun,
     EmployeePayrollRunsListRequestExpand,
     EmployeePayrollRunsRetrieveRequestExpand,
     EmployeeRequest,
+    EmployeeRequestEmploymentStatus,
+    EmployeeRequestEthnicity,
+    EmployeeRequestGender,
+    EmployeeRequestMaritalStatus,
     EmployeeResponse,
     EmployeesListRequestEmploymentStatus,
     EmployeesListRequestExpand,
     EmployeesListRequestRemoteFields,
     EmployeesListRequestShowEnumOrigins,
     EmployeesRetrieveRequestExpand,
     EmployeesRetrieveRequestRemoteFields,
     EmployeesRetrieveRequestShowEnumOrigins,
     Employment,
     EmploymentEmploymentType,
+    EmploymentFlsaStatus,
+    EmploymentPayCurrency,
+    EmploymentPayFrequency,
+    EmploymentPayPeriod,
     EmploymentStatusEnum,
     EmploymentTypeEnum,
     EmploymentsListRequestExpand,
     EmploymentsListRequestOrderBy,
     EmploymentsListRequestRemoteFields,
     EmploymentsListRequestShowEnumOrigins,
     EmploymentsRetrieveRequestExpand,
@@ -58,31 +70,34 @@
     EthnicityEnum,
     FlsaStatusEnum,
     GenderEnum,
     Group,
     GroupType,
     GroupTypeEnum,
     Issue,
+    IssueStatus,
     IssueStatusEnum,
     IssuesListRequestStatus,
     LinkToken,
     LinkedAccountCondition,
     LinkedAccountConditionRequest,
     LinkedAccountSelectiveSyncConfiguration,
     LinkedAccountSelectiveSyncConfigurationRequest,
     LinkedAccountStatus,
     LinkedAccountsListRequestCategory,
     Location,
+    LocationCountry,
     LocationLocationType,
     LocationTypeEnum,
     MaritalStatusEnum,
     MetaResponse,
     MethodEnum,
     ModelOperation,
     MultipartFormFieldRequest,
+    MultipartFormFieldRequestEncoding,
     OperatorSchema,
     PaginatedAccountDetailsAndActionsList,
     PaginatedBankInfoList,
     PaginatedBenefitList,
     PaginatedCompanyList,
     PaginatedConditionSchemaList,
     PaginatedEmployeeList,
@@ -98,14 +113,15 @@
     PaginatedTimeOffBalanceList,
     PaginatedTimeOffList,
     PayCurrencyEnum,
     PayFrequencyEnum,
     PayGroup,
     PayPeriodEnum,
     PayrollRun,
+    PayrollRunRunState,
     PayrollRunRunType,
     PayrollRunsListRequestRemoteFields,
     PayrollRunsListRequestRunType,
     PayrollRunsListRequestShowEnumOrigins,
     PayrollRunsRetrieveRequestRemoteFields,
     PayrollRunsRetrieveRequestShowEnumOrigins,
     PolicyTypeEnum,
@@ -131,20 +147,24 @@
     TimeOffListRequestExpand,
     TimeOffListRequestRemoteFields,
     TimeOffListRequestRequestType,
     TimeOffListRequestShowEnumOrigins,
     TimeOffListRequestStatus,
     TimeOffRequest,
     TimeOffRequestRequestType,
+    TimeOffRequestStatus,
     TimeOffRequestType,
+    TimeOffRequestUnits,
     TimeOffResponse,
     TimeOffRetrieveRequestExpand,
     TimeOffRetrieveRequestRemoteFields,
     TimeOffRetrieveRequestShowEnumOrigins,
+    TimeOffStatus,
     TimeOffStatusEnum,
+    TimeOffUnits,
     UnitsEnum,
     ValidationProblemSource,
     WarningValidationProblem,
     WebhookReceiver,
 )
 from .resources import (
     account_details,
@@ -201,28 +221,40 @@
     "DebugModeLog",
     "DebugModelLogSummary",
     "Deduction",
     "Earning",
     "EarningType",
     "EarningTypeEnum",
     "Employee",
+    "EmployeeEmploymentStatus",
+    "EmployeeEthnicity",
+    "EmployeeGender",
+    "EmployeeMaritalStatus",
     "EmployeePayrollRun",
     "EmployeePayrollRunsListRequestExpand",
     "EmployeePayrollRunsRetrieveRequestExpand",
     "EmployeeRequest",
+    "EmployeeRequestEmploymentStatus",
+    "EmployeeRequestEthnicity",
+    "EmployeeRequestGender",
+    "EmployeeRequestMaritalStatus",
     "EmployeeResponse",
     "EmployeesListRequestEmploymentStatus",
     "EmployeesListRequestExpand",
     "EmployeesListRequestRemoteFields",
     "EmployeesListRequestShowEnumOrigins",
     "EmployeesRetrieveRequestExpand",
     "EmployeesRetrieveRequestRemoteFields",
     "EmployeesRetrieveRequestShowEnumOrigins",
     "Employment",
     "EmploymentEmploymentType",
+    "EmploymentFlsaStatus",
+    "EmploymentPayCurrency",
+    "EmploymentPayFrequency",
+    "EmploymentPayPeriod",
     "EmploymentStatusEnum",
     "EmploymentTypeEnum",
     "EmploymentsListRequestExpand",
     "EmploymentsListRequestOrderBy",
     "EmploymentsListRequestRemoteFields",
     "EmploymentsListRequestShowEnumOrigins",
     "EmploymentsRetrieveRequestExpand",
@@ -234,31 +266,34 @@
     "EthnicityEnum",
     "FlsaStatusEnum",
     "GenderEnum",
     "Group",
     "GroupType",
     "GroupTypeEnum",
     "Issue",
+    "IssueStatus",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
     "LinkedAccountSelectiveSyncConfiguration",
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "Location",
+    "LocationCountry",
     "LocationLocationType",
     "LocationTypeEnum",
     "MaritalStatusEnum",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
+    "MultipartFormFieldRequestEncoding",
     "OperatorSchema",
     "PaginatedAccountDetailsAndActionsList",
     "PaginatedBankInfoList",
     "PaginatedBenefitList",
     "PaginatedCompanyList",
     "PaginatedConditionSchemaList",
     "PaginatedEmployeeList",
@@ -274,14 +309,15 @@
     "PaginatedTimeOffBalanceList",
     "PaginatedTimeOffList",
     "PayCurrencyEnum",
     "PayFrequencyEnum",
     "PayGroup",
     "PayPeriodEnum",
     "PayrollRun",
+    "PayrollRunRunState",
     "PayrollRunRunType",
     "PayrollRunsListRequestRemoteFields",
     "PayrollRunsListRequestRunType",
     "PayrollRunsListRequestShowEnumOrigins",
     "PayrollRunsRetrieveRequestRemoteFields",
     "PayrollRunsRetrieveRequestShowEnumOrigins",
     "PolicyTypeEnum",
@@ -307,20 +343,24 @@
     "TimeOffListRequestExpand",
     "TimeOffListRequestRemoteFields",
     "TimeOffListRequestRequestType",
     "TimeOffListRequestShowEnumOrigins",
     "TimeOffListRequestStatus",
     "TimeOffRequest",
     "TimeOffRequestRequestType",
+    "TimeOffRequestStatus",
     "TimeOffRequestType",
+    "TimeOffRequestUnits",
     "TimeOffResponse",
     "TimeOffRetrieveRequestExpand",
     "TimeOffRetrieveRequestRemoteFields",
     "TimeOffRetrieveRequestShowEnumOrigins",
+    "TimeOffStatus",
     "TimeOffStatusEnum",
+    "TimeOffUnits",
     "UnitsEnum",
     "ValidationProblemSource",
     "WarningValidationProblem",
     "WebhookReceiver",
     "account_details",
     "account_token",
     "available_actions",
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/__init__.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/account_details/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/account_details/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/account_token/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/account_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/available_actions/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/available_actions/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/bank_info/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/bank_info/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/benefits/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/benefits/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/companies/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/companies/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/delete_account/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/delete_account/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/employee_payroll_runs/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/employee_payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/employees/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/employees/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/employments/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/employments/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/force_resync/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/force_resync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/generate_key/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/generate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/groups/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/issues/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/issues/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/link_token/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/link_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/linked_accounts/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/linked_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/locations/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/locations/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/passthrough/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/passthrough/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/pay_groups/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/pay_groups/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/payroll_runs/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/payroll_runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/regenerate_key/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/regenerate_key/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/selective_sync/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/selective_sync/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/sync_status/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/sync_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/teams/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/teams/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/time_off/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/time_off/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/time_off_balances/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/time_off_balances/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/resources/webhook_receivers/client.py` & `fern_merge-0.0.29/src/merge/resources/hris/resources/webhook_receivers/client.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/__init__.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,40 @@
 from .debug_mode_log import DebugModeLog
 from .debug_model_log_summary import DebugModelLogSummary
 from .deduction import Deduction
 from .earning import Earning
 from .earning_type import EarningType
 from .earning_type_enum import EarningTypeEnum
 from .employee import Employee
+from .employee_employment_status import EmployeeEmploymentStatus
+from .employee_ethnicity import EmployeeEthnicity
+from .employee_gender import EmployeeGender
+from .employee_marital_status import EmployeeMaritalStatus
 from .employee_payroll_run import EmployeePayrollRun
 from .employee_payroll_runs_list_request_expand import EmployeePayrollRunsListRequestExpand
 from .employee_payroll_runs_retrieve_request_expand import EmployeePayrollRunsRetrieveRequestExpand
 from .employee_request import EmployeeRequest
+from .employee_request_employment_status import EmployeeRequestEmploymentStatus
+from .employee_request_ethnicity import EmployeeRequestEthnicity
+from .employee_request_gender import EmployeeRequestGender
+from .employee_request_marital_status import EmployeeRequestMaritalStatus
 from .employee_response import EmployeeResponse
 from .employees_list_request_employment_status import EmployeesListRequestEmploymentStatus
 from .employees_list_request_expand import EmployeesListRequestExpand
 from .employees_list_request_remote_fields import EmployeesListRequestRemoteFields
 from .employees_list_request_show_enum_origins import EmployeesListRequestShowEnumOrigins
 from .employees_retrieve_request_expand import EmployeesRetrieveRequestExpand
 from .employees_retrieve_request_remote_fields import EmployeesRetrieveRequestRemoteFields
 from .employees_retrieve_request_show_enum_origins import EmployeesRetrieveRequestShowEnumOrigins
 from .employment import Employment
 from .employment_employment_type import EmploymentEmploymentType
+from .employment_flsa_status import EmploymentFlsaStatus
+from .employment_pay_currency import EmploymentPayCurrency
+from .employment_pay_frequency import EmploymentPayFrequency
+from .employment_pay_period import EmploymentPayPeriod
 from .employment_status_enum import EmploymentStatusEnum
 from .employment_type_enum import EmploymentTypeEnum
 from .employments_list_request_expand import EmploymentsListRequestExpand
 from .employments_list_request_order_by import EmploymentsListRequestOrderBy
 from .employments_list_request_remote_fields import EmploymentsListRequestRemoteFields
 from .employments_list_request_show_enum_origins import EmploymentsListRequestShowEnumOrigins
 from .employments_retrieve_request_expand import EmploymentsRetrieveRequestExpand
@@ -57,31 +69,34 @@
 from .ethnicity_enum import EthnicityEnum
 from .flsa_status_enum import FlsaStatusEnum
 from .gender_enum import GenderEnum
 from .group import Group
 from .group_type import GroupType
 from .group_type_enum import GroupTypeEnum
 from .issue import Issue
+from .issue_status import IssueStatus
 from .issue_status_enum import IssueStatusEnum
 from .issues_list_request_status import IssuesListRequestStatus
 from .link_token import LinkToken
 from .linked_account_condition import LinkedAccountCondition
 from .linked_account_condition_request import LinkedAccountConditionRequest
 from .linked_account_selective_sync_configuration import LinkedAccountSelectiveSyncConfiguration
 from .linked_account_selective_sync_configuration_request import LinkedAccountSelectiveSyncConfigurationRequest
 from .linked_account_status import LinkedAccountStatus
 from .linked_accounts_list_request_category import LinkedAccountsListRequestCategory
 from .location import Location
+from .location_country import LocationCountry
 from .location_location_type import LocationLocationType
 from .location_type_enum import LocationTypeEnum
 from .marital_status_enum import MaritalStatusEnum
 from .meta_response import MetaResponse
 from .method_enum import MethodEnum
 from .model_operation import ModelOperation
 from .multipart_form_field_request import MultipartFormFieldRequest
+from .multipart_form_field_request_encoding import MultipartFormFieldRequestEncoding
 from .operator_schema import OperatorSchema
 from .paginated_account_details_and_actions_list import PaginatedAccountDetailsAndActionsList
 from .paginated_bank_info_list import PaginatedBankInfoList
 from .paginated_benefit_list import PaginatedBenefitList
 from .paginated_company_list import PaginatedCompanyList
 from .paginated_condition_schema_list import PaginatedConditionSchemaList
 from .paginated_employee_list import PaginatedEmployeeList
@@ -97,14 +112,15 @@
 from .paginated_time_off_balance_list import PaginatedTimeOffBalanceList
 from .paginated_time_off_list import PaginatedTimeOffList
 from .pay_currency_enum import PayCurrencyEnum
 from .pay_frequency_enum import PayFrequencyEnum
 from .pay_group import PayGroup
 from .pay_period_enum import PayPeriodEnum
 from .payroll_run import PayrollRun
+from .payroll_run_run_state import PayrollRunRunState
 from .payroll_run_run_type import PayrollRunRunType
 from .payroll_runs_list_request_remote_fields import PayrollRunsListRequestRemoteFields
 from .payroll_runs_list_request_run_type import PayrollRunsListRequestRunType
 from .payroll_runs_list_request_show_enum_origins import PayrollRunsListRequestShowEnumOrigins
 from .payroll_runs_retrieve_request_remote_fields import PayrollRunsRetrieveRequestRemoteFields
 from .payroll_runs_retrieve_request_show_enum_origins import PayrollRunsRetrieveRequestShowEnumOrigins
 from .policy_type_enum import PolicyTypeEnum
@@ -130,20 +146,24 @@
 from .time_off_list_request_expand import TimeOffListRequestExpand
 from .time_off_list_request_remote_fields import TimeOffListRequestRemoteFields
 from .time_off_list_request_request_type import TimeOffListRequestRequestType
 from .time_off_list_request_show_enum_origins import TimeOffListRequestShowEnumOrigins
 from .time_off_list_request_status import TimeOffListRequestStatus
 from .time_off_request import TimeOffRequest
 from .time_off_request_request_type import TimeOffRequestRequestType
+from .time_off_request_status import TimeOffRequestStatus
 from .time_off_request_type import TimeOffRequestType
+from .time_off_request_units import TimeOffRequestUnits
 from .time_off_response import TimeOffResponse
 from .time_off_retrieve_request_expand import TimeOffRetrieveRequestExpand
 from .time_off_retrieve_request_remote_fields import TimeOffRetrieveRequestRemoteFields
 from .time_off_retrieve_request_show_enum_origins import TimeOffRetrieveRequestShowEnumOrigins
+from .time_off_status import TimeOffStatus
 from .time_off_status_enum import TimeOffStatusEnum
+from .time_off_units import TimeOffUnits
 from .units_enum import UnitsEnum
 from .validation_problem_source import ValidationProblemSource
 from .warning_validation_problem import WarningValidationProblem
 from .webhook_receiver import WebhookReceiver
 
 __all__ = [
     "AccountDetails",
@@ -170,28 +190,40 @@
     "DebugModeLog",
     "DebugModelLogSummary",
     "Deduction",
     "Earning",
     "EarningType",
     "EarningTypeEnum",
     "Employee",
+    "EmployeeEmploymentStatus",
+    "EmployeeEthnicity",
+    "EmployeeGender",
+    "EmployeeMaritalStatus",
     "EmployeePayrollRun",
     "EmployeePayrollRunsListRequestExpand",
     "EmployeePayrollRunsRetrieveRequestExpand",
     "EmployeeRequest",
+    "EmployeeRequestEmploymentStatus",
+    "EmployeeRequestEthnicity",
+    "EmployeeRequestGender",
+    "EmployeeRequestMaritalStatus",
     "EmployeeResponse",
     "EmployeesListRequestEmploymentStatus",
     "EmployeesListRequestExpand",
     "EmployeesListRequestRemoteFields",
     "EmployeesListRequestShowEnumOrigins",
     "EmployeesRetrieveRequestExpand",
     "EmployeesRetrieveRequestRemoteFields",
     "EmployeesRetrieveRequestShowEnumOrigins",
     "Employment",
     "EmploymentEmploymentType",
+    "EmploymentFlsaStatus",
+    "EmploymentPayCurrency",
+    "EmploymentPayFrequency",
+    "EmploymentPayPeriod",
     "EmploymentStatusEnum",
     "EmploymentTypeEnum",
     "EmploymentsListRequestExpand",
     "EmploymentsListRequestOrderBy",
     "EmploymentsListRequestRemoteFields",
     "EmploymentsListRequestShowEnumOrigins",
     "EmploymentsRetrieveRequestExpand",
@@ -203,31 +235,34 @@
     "EthnicityEnum",
     "FlsaStatusEnum",
     "GenderEnum",
     "Group",
     "GroupType",
     "GroupTypeEnum",
     "Issue",
+    "IssueStatus",
     "IssueStatusEnum",
     "IssuesListRequestStatus",
     "LinkToken",
     "LinkedAccountCondition",
     "LinkedAccountConditionRequest",
     "LinkedAccountSelectiveSyncConfiguration",
     "LinkedAccountSelectiveSyncConfigurationRequest",
     "LinkedAccountStatus",
     "LinkedAccountsListRequestCategory",
     "Location",
+    "LocationCountry",
     "LocationLocationType",
     "LocationTypeEnum",
     "MaritalStatusEnum",
     "MetaResponse",
     "MethodEnum",
     "ModelOperation",
     "MultipartFormFieldRequest",
+    "MultipartFormFieldRequestEncoding",
     "OperatorSchema",
     "PaginatedAccountDetailsAndActionsList",
     "PaginatedBankInfoList",
     "PaginatedBenefitList",
     "PaginatedCompanyList",
     "PaginatedConditionSchemaList",
     "PaginatedEmployeeList",
@@ -243,14 +278,15 @@
     "PaginatedTimeOffBalanceList",
     "PaginatedTimeOffList",
     "PayCurrencyEnum",
     "PayFrequencyEnum",
     "PayGroup",
     "PayPeriodEnum",
     "PayrollRun",
+    "PayrollRunRunState",
     "PayrollRunRunType",
     "PayrollRunsListRequestRemoteFields",
     "PayrollRunsListRequestRunType",
     "PayrollRunsListRequestShowEnumOrigins",
     "PayrollRunsRetrieveRequestRemoteFields",
     "PayrollRunsRetrieveRequestShowEnumOrigins",
     "PolicyTypeEnum",
@@ -276,18 +312,22 @@
     "TimeOffListRequestExpand",
     "TimeOffListRequestRemoteFields",
     "TimeOffListRequestRequestType",
     "TimeOffListRequestShowEnumOrigins",
     "TimeOffListRequestStatus",
     "TimeOffRequest",
     "TimeOffRequestRequestType",
+    "TimeOffRequestStatus",
     "TimeOffRequestType",
+    "TimeOffRequestUnits",
     "TimeOffResponse",
     "TimeOffRetrieveRequestExpand",
     "TimeOffRetrieveRequestRemoteFields",
     "TimeOffRetrieveRequestShowEnumOrigins",
+    "TimeOffStatus",
     "TimeOffStatusEnum",
+    "TimeOffUnits",
     "UnitsEnum",
     "ValidationProblemSource",
     "WarningValidationProblem",
     "WebhookReceiver",
 ]
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_details.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_details.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_integration.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_details_and_actions_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_details_and_actions_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_integration.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_integration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_token.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/account_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/account_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/available_actions.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/available_actions.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/bank_info.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_account_type.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/bank_info_list_request_account_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/bank_info_list_request_order_by.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/bank_info_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/benefit.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/benefit.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/categories_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/categories_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/category_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/category_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/common_model_scopes_body_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/common_model_scopes_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/company.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/company.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/condition_schema.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/condition_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/condition_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/condition_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/country_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/country_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/debug_mode_log.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/debug_mode_log.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/debug_model_log_summary.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/debug_model_log_summary.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/deduction.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/deduction.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/earning.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/earning.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/earning_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/earning_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .employment_status_enum import EmploymentStatusEnum
-from .ethnicity_enum import EthnicityEnum
-from .gender_enum import GenderEnum
-from .marital_status_enum import MaritalStatusEnum
+from .employee_employment_status import EmployeeEmploymentStatus
+from .employee_ethnicity import EmployeeEthnicity
+from .employee_gender import EmployeeGender
+from .employee_marital_status import EmployeeMaritalStatus
 from .remote_data import RemoteData
 
 
 class Employee(pydantic.BaseModel):
     """
     # The Employee Object
     ### Description
@@ -46,40 +46,40 @@
     )
     home_location: typing.Optional[str] = pydantic.Field(description="The employee's home address.")
     work_location: typing.Optional[str] = pydantic.Field(description="The employee's work address.")
     manager: typing.Optional[str] = pydantic.Field(description="The employee ID of the employee's manager.")
     team: typing.Optional[str] = pydantic.Field(description="The employee's team.")
     pay_group: typing.Optional[str] = pydantic.Field(description="The employee's pay group")
     ssn: typing.Optional[str] = pydantic.Field(description="The employee's social security number.")
-    gender: typing.Optional[GenderEnum] = pydantic.Field(
+    gender: typing.Optional[EmployeeGender] = pydantic.Field(
         description=(
             "The employee's gender.\n"
             "\n"
             "* `MALE` - MALE\n"
             "* `FEMALE` - FEMALE\n"
             "* `NON-BINARY` - NON-BINARY\n"
             "* `OTHER` - OTHER\n"
             "* `PREFER_NOT_TO_DISCLOSE` - PREFER_NOT_TO_DISCLOSE\n"
         )
     )
-    ethnicity: typing.Optional[EthnicityEnum] = pydantic.Field(
+    ethnicity: typing.Optional[EmployeeEthnicity] = pydantic.Field(
         description=(
             "The employee's ethnicity.\n"
             "\n"
             "* `AMERICAN_INDIAN_OR_ALASKA_NATIVE` - AMERICAN_INDIAN_OR_ALASKA_NATIVE\n"
             "* `ASIAN_OR_INDIAN_SUBCONTINENT` - ASIAN_OR_INDIAN_SUBCONTINENT\n"
             "* `BLACK_OR_AFRICAN_AMERICAN` - BLACK_OR_AFRICAN_AMERICAN\n"
             "* `HISPANIC_OR_LATINO` - HISPANIC_OR_LATINO\n"
             "* `NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER` - NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER\n"
             "* `TWO_OR_MORE_RACES` - TWO_OR_MORE_RACES\n"
             "* `WHITE` - WHITE\n"
             "* `PREFER_NOT_TO_DISCLOSE` - PREFER_NOT_TO_DISCLOSE\n"
         )
     )
-    marital_status: typing.Optional[MaritalStatusEnum] = pydantic.Field(
+    marital_status: typing.Optional[EmployeeMaritalStatus] = pydantic.Field(
         description=(
             "The employee's filing status as related to marital status.\n"
             "\n"
             "* `SINGLE` - SINGLE\n"
             "* `MARRIED_FILING_JOINTLY` - MARRIED_FILING_JOINTLY\n"
             "* `MARRIED_FILING_SEPARATELY` - MARRIED_FILING_SEPARATELY\n"
             "* `HEAD_OF_HOUSEHOLD` - HEAD_OF_HOUSEHOLD\n"
@@ -90,15 +90,15 @@
     hire_date: typing.Optional[str] = pydantic.Field(
         description="The date that the employee was hired, usually the day that an offer letter is signed. If an employee has multiple hire dates from previous employments, this represents the most recent hire date. Note: If you're looking for the employee's start date, refer to the start_date field."
     )
     start_date: typing.Optional[str] = pydantic.Field(
         description="The date that the employee started working. If an employee was rehired, the most recent start date will be returned."
     )
     remote_created_at: typing.Optional[str] = pydantic.Field(description="When the third party's employee was created.")
-    employment_status: typing.Optional[EmploymentStatusEnum] = pydantic.Field(
+    employment_status: typing.Optional[EmployeeEmploymentStatus] = pydantic.Field(
         description=(
             "The employment status of the employee.\n"
             "\n"
             "* `ACTIVE` - ACTIVE\n"
             "* `PENDING` - PENDING\n"
             "* `INACTIVE` - INACTIVE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_run.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_run.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_runs_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee_payroll_runs_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .employment_status_enum import EmploymentStatusEnum
-from .ethnicity_enum import EthnicityEnum
-from .gender_enum import GenderEnum
-from .marital_status_enum import MaritalStatusEnum
+from .employee_request_employment_status import EmployeeRequestEmploymentStatus
+from .employee_request_ethnicity import EmployeeRequestEthnicity
+from .employee_request_gender import EmployeeRequestGender
+from .employee_request_marital_status import EmployeeRequestMaritalStatus
 
 
 class EmployeeRequest(pydantic.BaseModel):
     """
     # The Employee Object
     ### Description
     The `Employee` object is used to represent any person who has been employed by a company.
@@ -43,40 +43,40 @@
     )
     home_location: typing.Optional[str] = pydantic.Field(description="The employee's home address.")
     work_location: typing.Optional[str] = pydantic.Field(description="The employee's work address.")
     manager: typing.Optional[str] = pydantic.Field(description="The employee ID of the employee's manager.")
     team: typing.Optional[str] = pydantic.Field(description="The employee's team.")
     pay_group: typing.Optional[str] = pydantic.Field(description="The employee's pay group")
     ssn: typing.Optional[str] = pydantic.Field(description="The employee's social security number.")
-    gender: typing.Optional[GenderEnum] = pydantic.Field(
+    gender: typing.Optional[EmployeeRequestGender] = pydantic.Field(
         description=(
             "The employee's gender.\n"
             "\n"
             "* `MALE` - MALE\n"
             "* `FEMALE` - FEMALE\n"
             "* `NON-BINARY` - NON-BINARY\n"
             "* `OTHER` - OTHER\n"
             "* `PREFER_NOT_TO_DISCLOSE` - PREFER_NOT_TO_DISCLOSE\n"
         )
     )
-    ethnicity: typing.Optional[EthnicityEnum] = pydantic.Field(
+    ethnicity: typing.Optional[EmployeeRequestEthnicity] = pydantic.Field(
         description=(
             "The employee's ethnicity.\n"
             "\n"
             "* `AMERICAN_INDIAN_OR_ALASKA_NATIVE` - AMERICAN_INDIAN_OR_ALASKA_NATIVE\n"
             "* `ASIAN_OR_INDIAN_SUBCONTINENT` - ASIAN_OR_INDIAN_SUBCONTINENT\n"
             "* `BLACK_OR_AFRICAN_AMERICAN` - BLACK_OR_AFRICAN_AMERICAN\n"
             "* `HISPANIC_OR_LATINO` - HISPANIC_OR_LATINO\n"
             "* `NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER` - NATIVE_HAWAIIAN_OR_OTHER_PACIFIC_ISLANDER\n"
             "* `TWO_OR_MORE_RACES` - TWO_OR_MORE_RACES\n"
             "* `WHITE` - WHITE\n"
             "* `PREFER_NOT_TO_DISCLOSE` - PREFER_NOT_TO_DISCLOSE\n"
         )
     )
-    marital_status: typing.Optional[MaritalStatusEnum] = pydantic.Field(
+    marital_status: typing.Optional[EmployeeRequestMaritalStatus] = pydantic.Field(
         description=(
             "The employee's filing status as related to marital status.\n"
             "\n"
             "* `SINGLE` - SINGLE\n"
             "* `MARRIED_FILING_JOINTLY` - MARRIED_FILING_JOINTLY\n"
             "* `MARRIED_FILING_SEPARATELY` - MARRIED_FILING_SEPARATELY\n"
             "* `HEAD_OF_HOUSEHOLD` - HEAD_OF_HOUSEHOLD\n"
@@ -86,15 +86,15 @@
     date_of_birth: typing.Optional[str] = pydantic.Field(description="The employee's date of birth.")
     hire_date: typing.Optional[str] = pydantic.Field(
         description="The date that the employee was hired, usually the day that an offer letter is signed. If an employee has multiple hire dates from previous employments, this represents the most recent hire date. Note: If you're looking for the employee's start date, refer to the start_date field."
     )
     start_date: typing.Optional[str] = pydantic.Field(
         description="The date that the employee started working. If an employee was rehired, the most recent start date will be returned."
     )
-    employment_status: typing.Optional[EmploymentStatusEnum] = pydantic.Field(
+    employment_status: typing.Optional[EmployeeRequestEmploymentStatus] = pydantic.Field(
         description=(
             "The employment status of the employee.\n"
             "\n"
             "* `ACTIVE` - ACTIVE\n"
             "* `PENDING` - PENDING\n"
             "* `INACTIVE` - INACTIVE\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employee_response.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employee_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_employment_status.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_employment_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employees_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employment.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employment.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .employment_employment_type import EmploymentEmploymentType
-from .flsa_status_enum import FlsaStatusEnum
-from .pay_currency_enum import PayCurrencyEnum
-from .pay_frequency_enum import PayFrequencyEnum
-from .pay_period_enum import PayPeriodEnum
+from .employment_flsa_status import EmploymentFlsaStatus
+from .employment_pay_currency import EmploymentPayCurrency
+from .employment_pay_frequency import EmploymentPayFrequency
+from .employment_pay_period import EmploymentPayPeriod
 from .remote_data import RemoteData
 
 
 class Employment(pydantic.BaseModel):
     """
     # The Employment Object
     ### Description
@@ -27,45 +27,45 @@
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     employee: typing.Optional[str] = pydantic.Field(description="The employee holding this position.")
     job_title: typing.Optional[str] = pydantic.Field(description="The position's title.")
     pay_rate: typing.Optional[float] = pydantic.Field(description="The position's pay rate in dollars.")
-    pay_period: typing.Optional[PayPeriodEnum] = pydantic.Field(
+    pay_period: typing.Optional[EmploymentPayPeriod] = pydantic.Field(
         description=(
             "The time period this pay rate encompasses.\n"
             "\n"
             "* `HOUR` - HOUR\n"
             "* `DAY` - DAY\n"
             "* `WEEK` - WEEK\n"
             "* `EVERY_TWO_WEEKS` - EVERY_TWO_WEEKS\n"
             "* `SEMIMONTHLY` - SEMIMONTHLY\n"
             "* `MONTH` - MONTH\n"
             "* `QUARTER` - QUARTER\n"
             "* `EVERY_SIX_MONTHS` - EVERY_SIX_MONTHS\n"
             "* `YEAR` - YEAR\n"
         )
     )
-    pay_frequency: typing.Optional[PayFrequencyEnum] = pydantic.Field(
+    pay_frequency: typing.Optional[EmploymentPayFrequency] = pydantic.Field(
         description=(
             "The position's pay frequency.\n"
             "\n"
             "* `WEEKLY` - WEEKLY\n"
             "* `BIWEEKLY` - BIWEEKLY\n"
             "* `MONTHLY` - MONTHLY\n"
             "* `QUARTERLY` - QUARTERLY\n"
             "* `SEMIANNUALLY` - SEMIANNUALLY\n"
             "* `ANNUALLY` - ANNUALLY\n"
             "* `THIRTEEN-MONTHLY` - THIRTEEN-MONTHLY\n"
             "* `PRO_RATA` - PRO_RATA\n"
             "* `SEMIMONTHLY` - SEMIMONTHLY\n"
         )
     )
-    pay_currency: typing.Optional[PayCurrencyEnum] = pydantic.Field(
+    pay_currency: typing.Optional[EmploymentPayCurrency] = pydantic.Field(
         description=(
             "The position's currency code.\n"
             "\n"
             "* `XUA` - ADB Unit of Account\n"
             "* `AFN` - Afghan Afghani\n"
             "* `AFA` - Afghan Afghani (1927–2002)\n"
             "* `ALL` - Albanian Lek\n"
@@ -370,15 +370,15 @@
             "* `ZMK` - Zambian Kwacha (1968–2012)\n"
             "* `ZWD` - Zimbabwean Dollar (1980–2008)\n"
             "* `ZWR` - Zimbabwean Dollar (2008)\n"
             "* `ZWL` - Zimbabwean Dollar (2009)\n"
         )
     )
     pay_group: typing.Optional[str] = pydantic.Field(description="The employment's pay group")
-    flsa_status: typing.Optional[FlsaStatusEnum] = pydantic.Field(
+    flsa_status: typing.Optional[EmploymentFlsaStatus] = pydantic.Field(
         description=(
             "The position's FLSA status.\n"
             "\n"
             "* `EXEMPT` - EXEMPT\n"
             "* `SALARIED_NONEXEMPT` - SALARIED_NONEXEMPT\n"
             "* `NONEXEMPT` - NONEXEMPT\n"
             "* `OWNER` - OWNER\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employment_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employment_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employment_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employment_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_order_by.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_order_by.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/employments_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/enabled_actions_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/enabled_actions_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/encoding_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/encoding_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/error_validation_problem.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/error_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/ethnicity_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/ethnicity_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/flsa_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/flsa_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/gender_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/gender_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/group.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/group_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/group_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/issue.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .issue_status_enum import IssueStatusEnum
+from .issue_status import IssueStatus
 
 
 class Issue(pydantic.BaseModel):
     id: typing.Optional[str]
-    status: typing.Optional[IssueStatusEnum] = pydantic.Field(
+    status: typing.Optional[IssueStatus] = pydantic.Field(
         description=(
             "Status of the issue. Options: ('ONGOING', 'RESOLVED')\n"
             "\n"
             "* `ONGOING` - ONGOING\n"
             "* `RESOLVED` - RESOLVED\n"
         )
     )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/issue_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/issue_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/link_token.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/link_token.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_condition.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_condition_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_condition_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_selective_sync_configuration.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_selective_sync_configuration_request.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_account_status.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_account_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/linked_accounts_list_request_category.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/linked_accounts_list_request_category.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/location.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .country_enum import CountryEnum
+from .location_country import LocationCountry
 from .location_location_type import LocationLocationType
 from .remote_data import RemoteData
 
 
 class Location(pydantic.BaseModel):
     """
     # The Location Object
@@ -28,15 +28,15 @@
     street_1: typing.Optional[str] = pydantic.Field(description="Line 1 of the location's street address.")
     street_2: typing.Optional[str] = pydantic.Field(description="Line 2 of the location's street address.")
     city: typing.Optional[str] = pydantic.Field(description="The location's city.")
     state: typing.Optional[str] = pydantic.Field(
         description="The location's state. Represents a region if outside of the US."
     )
     zip_code: typing.Optional[str] = pydantic.Field(description="The location's zip code or postal code.")
-    country: typing.Optional[CountryEnum] = pydantic.Field(
+    country: typing.Optional[LocationCountry] = pydantic.Field(
         description=(
             "The location's country.\n"
             "\n"
             "* `AF` - Afghanistan\n"
             "* `AX` - Åland Islands\n"
             "* `AL` - Albania\n"
             "* `DZ` - Algeria\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/marital_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/marital_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/meta_response.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/method_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/method_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/model_operation.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/model_operation.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/multipart_form_field_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/multipart_form_field_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .encoding_enum import EncodingEnum
+from .multipart_form_field_request_encoding import MultipartFormFieldRequestEncoding
 
 
 class MultipartFormFieldRequest(pydantic.BaseModel):
     """
     # The MultipartFormField Object
     ### Description
     The `MultipartFormField` object is used to represent fields in an HTTP request using `multipart/form-data`.
@@ -21,15 +21,15 @@
 
     name: str = pydantic.Field(
         description='The name of the form field <span style="white-space: nowrap">`non-empty`</span> '
     )
     data: str = pydantic.Field(
         description='The data for the form field. <span style="white-space: nowrap">`non-empty`</span> '
     )
-    encoding: typing.Optional[EncodingEnum] = pydantic.Field(
+    encoding: typing.Optional[MultipartFormFieldRequestEncoding] = pydantic.Field(
         description=(
             "The encoding of the value of `data`. Defaults to `RAW` if not defined.\n"
             "\n"
             "* `RAW` - RAW\n"
             "* `BASE64` - BASE64\n"
             "* `GZIP_BASE64` - GZIP_BASE64\n"
         )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/operator_schema.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/operator_schema.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_account_details_and_actions_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_bank_info_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_bank_info_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_benefit_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_benefit_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_company_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_condition_schema_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_condition_schema_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employee_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employee_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_employment_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_employment_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_group_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_issue_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_issue_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_location_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_location_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_pay_group_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_pay_group_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_payroll_run_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_payroll_run_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_sync_status_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_sync_status_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_team_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_balance_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_time_off_balance_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/paginated_time_off_list.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/paginated_time_off_list.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/pay_currency_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/pay_currency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/pay_frequency_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/pay_frequency_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/pay_group.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/pay_group.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/pay_period_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/pay_period_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_run.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .payroll_run_run_state import PayrollRunRunState
 from .payroll_run_run_type import PayrollRunRunType
 from .remote_data import RemoteData
-from .run_state_enum import RunStateEnum
 
 
 class PayrollRun(pydantic.BaseModel):
     """
     # The PayrollRun Object
     ### Description
     The `PayrollRun` object is used to represent a group of pay statements for a specific pay schedule.
 
     ### Usage Example
     Fetch from the `LIST PayrollRuns` endpoint and filter by `ID` to show all payroll runs.
     """
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
-    run_state: typing.Optional[RunStateEnum] = pydantic.Field(
+    run_state: typing.Optional[PayrollRunRunState] = pydantic.Field(
         description=(
             "The state of the payroll run\n"
             "\n"
             "* `PAID` - PAID\n"
             "* `DRAFT` - DRAFT\n"
             "* `APPROVED` - APPROVED\n"
             "* `FAILED` - FAILED\n"
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_run_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/payroll_runs_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/policy_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/policy_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/reason_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/reason_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/remote_data.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/remote_data.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/remote_key.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/remote_key.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/remote_response.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/remote_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/request_format_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/request_format_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/request_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/request_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/response_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/response_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/run_state_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/run_state_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/run_type_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/run_type_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/selective_sync_configurations_usage_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/sync_status.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/sync_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/sync_status_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/sync_status_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/tax.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/tax.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/team.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/team.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .remote_data import RemoteData
 from .time_off_request_type import TimeOffRequestType
-from .time_off_status_enum import TimeOffStatusEnum
-from .units_enum import UnitsEnum
+from .time_off_status import TimeOffStatus
+from .time_off_units import TimeOffUnits
 
 
 class TimeOff(pydantic.BaseModel):
     """
     # The TimeOff Object
     ### Description
     The `TimeOff` object is used to represent all employees' Time Off entries.
@@ -24,27 +24,27 @@
 
     id: typing.Optional[str]
     remote_id: typing.Optional[str] = pydantic.Field(description="The third-party API ID of the matching object.")
     employee: typing.Optional[str] = pydantic.Field(description="The employee requesting time off.")
     approver: typing.Optional[str] = pydantic.Field(
         description="The Merge ID of the employee with the ability to approve the time off request."
     )
-    status: typing.Optional[TimeOffStatusEnum] = pydantic.Field(
+    status: typing.Optional[TimeOffStatus] = pydantic.Field(
         description=(
             "The status of this time off request.\n"
             "\n"
             "* `REQUESTED` - REQUESTED\n"
             "* `APPROVED` - APPROVED\n"
             "* `DECLINED` - DECLINED\n"
             "* `CANCELLED` - CANCELLED\n"
             "* `DELETED` - DELETED\n"
         )
     )
     employee_note: typing.Optional[str] = pydantic.Field(description="The employee note for this time off request.")
-    units: typing.Optional[UnitsEnum] = pydantic.Field(
+    units: typing.Optional[TimeOffUnits] = pydantic.Field(
         description=(
             "The measurement that the third-party integration uses to count time requested.\n"
             "\n"
             "* `HOURS` - HOURS\n"
             "* `DAYS` - DAYS\n"
         )
     )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balance.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_balance.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_balances_list_request_policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_request_type.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_request_type.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_list_request_status.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_list_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_request.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .time_off_request_request_type import TimeOffRequestRequestType
-from .time_off_status_enum import TimeOffStatusEnum
-from .units_enum import UnitsEnum
+from .time_off_request_status import TimeOffRequestStatus
+from .time_off_request_units import TimeOffRequestUnits
 
 
 class TimeOffRequest(pydantic.BaseModel):
     """
     # The TimeOff Object
     ### Description
     The `TimeOff` object is used to represent all employees' Time Off entries.
@@ -21,27 +21,27 @@
     Fetch from the `LIST TimeOffs` endpoint and filter by `ID` to show all time off requests.
     """
 
     employee: typing.Optional[str] = pydantic.Field(description="The employee requesting time off.")
     approver: typing.Optional[str] = pydantic.Field(
         description="The Merge ID of the employee with the ability to approve the time off request."
     )
-    status: typing.Optional[TimeOffStatusEnum] = pydantic.Field(
+    status: typing.Optional[TimeOffRequestStatus] = pydantic.Field(
         description=(
             "The status of this time off request.\n"
             "\n"
             "* `REQUESTED` - REQUESTED\n"
             "* `APPROVED` - APPROVED\n"
             "* `DECLINED` - DECLINED\n"
             "* `CANCELLED` - CANCELLED\n"
             "* `DELETED` - DELETED\n"
         )
     )
     employee_note: typing.Optional[str] = pydantic.Field(description="The employee note for this time off request.")
-    units: typing.Optional[UnitsEnum] = pydantic.Field(
+    units: typing.Optional[TimeOffRequestUnits] = pydantic.Field(
         description=(
             "The measurement that the third-party integration uses to count time requested.\n"
             "\n"
             "* `HOURS` - HOURS\n"
             "* `DAYS` - DAYS\n"
         )
     )
```

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_response.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_response.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_expand.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_expand.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_remote_fields.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_retrieve_request_show_enum_origins.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/time_off_status_enum.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/time_off_status_enum.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/validation_problem_source.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/validation_problem_source.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/warning_validation_problem.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/warning_validation_problem.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/src/merge/resources/hris/types/webhook_receiver.py` & `fern_merge-0.0.29/src/merge/resources/hris/types/webhook_receiver.py`

 * *Files identical despite different names*

### Comparing `fern_merge-0.0.28/PKG-INFO` & `fern_merge-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-merge
-Version: 0.0.28
+Version: 0.0.29
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

