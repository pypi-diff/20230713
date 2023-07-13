# Comparing `tmp/castoredc_api-0.1.8.tar.gz` & `tmp/castoredc_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castoredc_api-0.1.8.tar", last modified: Wed Apr 26 07:36:11 2023, max compression
+gzip compressed data, was "castoredc_api-0.1.9.tar", last modified: Thu Jul 13 09:59:31 2023, max compression
```

## Comparing `castoredc_api-0.1.8.tar` & `castoredc_api-0.1.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-04-26 07:36:11.779252 castoredc_api-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/auth/auth_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53662 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/castoredc_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/client_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/importer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/async_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    27909 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/sync_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/study/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/study/castor_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_report_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_study_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_survey_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    44398 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/data_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/fixtures_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/fixtures_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38852 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/data_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/fixtures_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_structure_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_special_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_structure_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_archived.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 07:36:11.779252 castoredc_api-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.106408 castoredc_api-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-07-13 09:59:31.110408 castoredc_api-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.090408 castoredc_api-0.1.9/castoredc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.090408 castoredc_api-0.1.9/castoredc_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/auth/auth_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.090408 castoredc_api-0.1.9/castoredc_api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54574 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/client/castoredc_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/client/client_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.094408 castoredc_api-0.1.9/castoredc_api/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/async_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27909 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/importer/sync_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.094408 castoredc_api-0.1.9/castoredc_api/study/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.094408 castoredc_api-0.1.9/castoredc_api/study/castor_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_report_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_study_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_survey_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44232 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/study/castor_study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.094408 castoredc_api-0.1.9/castoredc_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.102408 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/fixtures_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25554 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.102408 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.102408 castoredc_api-0.1.9/castoredc_api/tests/test_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/fixtures_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.102408 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.106408 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38852 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.106408 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.106408 castoredc_api-0.1.9/castoredc_api/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/data_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/fixtures_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_structure_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_special_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_structure_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.106408 castoredc_api-0.1.9/castoredc_api/tests/test_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output_archived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:31.090408 castoredc_api-0.1.9/castoredc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-07-13 09:59:31.000000 castoredc_api-0.1.9/castoredc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-13 09:59:31.000000 castoredc_api-0.1.9/castoredc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:59:31.000000 castoredc_api-0.1.9/castoredc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 09:59:31.000000 castoredc_api-0.1.9/castoredc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 09:59:31.000000 castoredc_api-0.1.9/castoredc_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 09:59:31.110408 castoredc_api-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-13 09:58:55.000000 castoredc_api-0.1.9/setup.py
```

### Comparing `castoredc_api-0.1.8/LICENSE.md` & `castoredc_api-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/PKG-INFO` & `castoredc_api-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castoredc_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for the Castor EDC API
 Home-page: https://github.com/reiniervlinschoten/castoredc_api
 Author: Reinier van Linschoten
 Author-email: mail@reiniervl.com
 Maintainer: Reinier van Linschoten
 Maintainer-email: mail@reiniervl.com
 License: MIT
@@ -19,15 +19,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2023.1
+#### Supports CastorEDC Release 2023.2
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.8/README.md` & `castoredc_api-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2023.1
+#### Supports CastorEDC Release 2023.2
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.8/castoredc_api/client/castoredc_api_client.py` & `castoredc_api-0.1.9/castoredc_api/client/castoredc_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -870,14 +870,30 @@
             "email": email,
             "message": message,
             "manage_permission": manage_permissions,
             "institute_permissions": institute_permissions,
         }
         return self.sync_post(url, body)
 
+    def delete_user_study(self, study_id, user_id):
+        """Deletes a user from the study."""
+        url = self.base_url + f"/study/{study_id}/user/{user_id}"
+        return self.sync_delete(url, params={})
+
+    def update_permissions_user_study(
+        self, study_id, user_id, manage_permissions, site_permissions
+    ):
+        """Updates permissions for a user."""
+        url = self.base_url + f"/study/{study_id}/user/{user_id}"
+        body = {
+            "manage_permissions": manage_permissions,
+            "site_permissions": site_permissions,
+        }
+        return self.sync_put(url, body)
+
     # STUDY-DATA-ENTRY
     @RateLimiter(**client_options.SYNC_OPTIONS)
     def all_study_fields_record(self, record_id):
         """Returns a list of all study fields of a record.
         Returns None if record not found."""
         endpoint = f"/record/{record_id}/data-point/study"
         return self.retrieve_all_data_by_endpoint(endpoint, data_name="StudyDataPoints")
@@ -1281,15 +1297,22 @@
         response.raise_for_status()
         return response.json()
 
     def sync_delete(self, url, params: dict):
         """Helper function to send delete to url."""
         response = self.client.delete(url=url, params=params)
         response.raise_for_status()
-        return response.json()
+        return {"code": response.status_code}
+
+    def sync_put(self, url, body: dict):
+        """Helper function to send put to url."""
+        response = self.client.put(url=url, json=body)
+        print(response.json())
+        response.raise_for_status()
+        return {"code": response.status_code, "json": response.json()}
 
     # Asynchronous API Interaction
     async def async_get(self, url: str, params: list) -> list:
         """Queries the Castor EDC API on given url with parameters params.
         Queries the database once for each parameter dict in the params list.
         Returns a list of responses.
```

### Comparing `castoredc_api-0.1.8/castoredc_api/client/client_options.py` & `castoredc_api-0.1.9/castoredc_api/client/client_options.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/importer/async_helpers.py` & `castoredc_api-0.1.9/castoredc_api/importer/async_helpers.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/importer/async_import.py` & `castoredc_api-0.1.9/castoredc_api/importer/async_import.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/importer/helpers.py` & `castoredc_api-0.1.9/castoredc_api/importer/helpers.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/importer/import_data.py` & `castoredc_api-0.1.9/castoredc_api/importer/import_data.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/importer/sync_import.py` & `castoredc_api-0.1.9/castoredc_api/importer/sync_import.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_data_point.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_data_point.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_field.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_field.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_form.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form_instance.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_record.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_record.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_report_form_instance.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_report_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_step.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_step.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_study_form_instance.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_study_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_survey_form_instance.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_objects/castor_survey_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/study/castor_study.py` & `castoredc_api-0.1.9/castoredc_api/study/castor_study.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,17 +308,15 @@
         }
         for child_id in dependencies:
             self.get_single_field(child_id).field_dependency = dependencies[child_id]
 
     # DATA ANALYSIS
     def export_to_dataframe(self, archived=False) -> dict:
         """Exports all data from a study into a dict of dataframes for statistical analysis."""
-        # TODO: change this to the correct archived, # pylint: disable=fixme
-        #  fails now because the parameter does not seem to be handled correctly server side
-        self.map_data(archived=True)
+        self.map_data(archived=archived)
         dataframes = {
             "Study": self.__export_study_data(archived),
             "Surveys": self.__export_survey_data(archived),
             "Reports": self.__export_report_data(archived),
         }
         return dataframes
```

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/data_models.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/data_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,15 @@
     "created_by": [
         str,
     ],
     "sent_on": [dict, type(None)],
     "received_on": [dict, type(None)],
     "first_opened_on": [dict, type(None)],
     "finished_on": [dict, type(None)],
-    "available_from": [dict],
+    "available_from": [dict, type(None)],
     "expire_on": [str, type(None)],
     "all_fields_filled_on": [dict, type(None)],
     "started_on": [dict, type(None)],
     "locked": [
         bool,
     ],
     "archived": [
```

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/fixtures_api.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,19 +122,15 @@
         "invitation_content": 'Dear participant,\n\nYou are participating in the study "Example Study" and we would like to ask you to fill in a survey.\n\nPlease click the link below to complete our survey.\n\n{url}\n\n{logo}',
         "created_on": {
             "date": "2019-10-14 09:42:27.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "created_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
-        "available_from": {
-            "date": "2019-10-14 09:42:27.000000",
-            "timezone_type": 3,
-            "timezone": "Europe/Amsterdam",
-        },
+        "available_from": None,
         "expire_on": None,
         "sent_on": None,
         "first_opened_on": None,
         "started_on": None,
         "all_fields_filled_on": None,
         "finished_on": {
             "date": "2020-08-14 16:27:12.000000",
```

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_data_point.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_data_point.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_field.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_field.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_form.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_record.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_record.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_step.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_step.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_study.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_castor_objects/test_castor_study.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_client.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/data_ids.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/data_ids.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/fixtures_integration.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/fixtures_integration.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_interpretation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_mapping.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_mapping.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_structure_mapping.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_data_structure_mapping.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_special_cases.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_special_cases.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_structure_mapping.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_integration/test_structure_mapping.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_archived.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output_archived.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_format.py` & `castoredc_api-0.1.9/castoredc_api/tests/test_output/test_csv_output_format.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/castoredc_api.egg-info/PKG-INFO` & `castoredc_api-0.1.9/castoredc_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castoredc-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for the Castor EDC API
 Home-page: https://github.com/reiniervlinschoten/castoredc_api
 Author: Reinier van Linschoten
 Author-email: mail@reiniervl.com
 Maintainer: Reinier van Linschoten
 Maintainer-email: mail@reiniervl.com
 License: MIT
@@ -19,15 +19,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2023.1
+#### Supports CastorEDC Release 2023.2
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.8/castoredc_api.egg-info/SOURCES.txt` & `castoredc_api-0.1.9/castoredc_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.8/setup.py` & `castoredc_api-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="castoredc_api",
-    version="0.1.8",
+    version="0.1.9",
     description="Python wrapper for the Castor EDC API",
     author="Reinier van Linschoten",
     author_email="mail@reiniervl.com",
     maintainer="Reinier van Linschoten",
     maintainer_email="mail@reiniervl.com",
     url="https://github.com/reiniervlinschoten/castoredc_api",
     packages=find_packages(include=("castoredc_api", "castoredc_api.*")),
```

