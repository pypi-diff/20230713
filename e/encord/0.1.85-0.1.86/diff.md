# Comparing `tmp/encord-0.1.85.tar.gz` & `tmp/encord-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.85.tar", max compression
+gzip compressed data, was "encord-0.1.86.tar", max compression
```

## Comparing `encord-0.1.85.tar` & `encord-0.1.86.tar`

### file list

```diff
@@ -1,90 +1,89 @@
--rw-r--r--   0        0        0    11330 2023-07-04 16:11:17.923206 encord-0.1.85/LICENSE
--rw-r--r--   0        0        0     2037 2023-07-04 16:11:17.923206 encord-0.1.85/README.md
--rw-r--r--   0        0        0       84 2023-07-04 16:11:17.923206 encord-0.1.85/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-07-04 16:11:17.939206 encord-0.1.85/encord/__init__.py
--rw-r--r--   0        0        0      240 2023-07-04 16:11:17.939206 encord-0.1.85/encord/_version.py
--rw-r--r--   0        0        0    49540 2023-07-04 16:11:17.939206 encord-0.1.85/encord/client.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/__init__.py
--rw-r--r--   0        0        0       45 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/constants.py
--rw-r--r--   0        0        0      464 2023-07-04 16:11:17.939206 encord-0.1.85/encord/common/enum.py
--rw-r--r--   0        0        0    10852 2023-07-04 16:11:17.939206 encord-0.1.85/encord/configs.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/__init__.py
--rw-r--r--   0        0        0      866 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/enums.py
--rw-r--r--   0        0        0     3196 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/model.py
--rw-r--r--   0        0        0     4522 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-07-04 16:11:17.939206 encord-0.1.85/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-07-04 16:11:17.939206 encord-0.1.85/encord/dataset.py
--rw-r--r--   0        0        0     6355 2023-07-04 16:11:17.939206 encord-0.1.85/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/bundle.py
--rw-r--r--   0        0        0      319 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/common.py
--rw-r--r--   0        0        0      535 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/limits.py
--rw-r--r--   0        0        0     7870 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/querier.py
--rw-r--r--   0        0        0      747 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/query_methods.py
--rw-r--r--   0        0        0     1738 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/__init__.py
--rw-r--r--   0        0        0     3447 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/api_client.py
--rw-r--r--   0        0        0      964 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/error_utils.py
--rw-r--r--   0        0        0      216 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/payloads.py
--rw-r--r--   0        0        0     2249 2023-07-04 16:11:17.939206 encord-0.1.85/encord/http/v2/request_signer.py
--rw-r--r--   0        0        0      340 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/classification.py
--rw-r--r--   0        0        0    21796 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/frames.py
--rw-r--r--   0        0        0    21928 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   140254 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/project.py
--rw-r--r--   0        0        0     1622 2023-07-04 16:11:17.939206 encord-0.1.85/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-07-04 16:11:17.939206 encord-0.1.85/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/__init__.py
--rw-r--r--   0        0        0      932 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/analytics.py
--rw-r--r--   0        0        0      982 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/api_key.py
--rw-r--r--   0        0        0      626 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/__init__.py
--rw-r--r--   0        0        0      337 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/base_dto_interface.py
--rw-r--r--   0        0        0     1418 2023-07-04 16:11:17.939206 encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v1.py
--rw-r--r--   0        0        0     1366 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v2.py
--rw-r--r--   0        0        0     5335 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32857 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/dataset.py
--rw-r--r--   0        0        0      829 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      256 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/formatter.py
--rw-r--r--   0        0        0     1241 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/label_log.py
--rw-r--r--   0        0        0    11889 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6679 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/model.py
--rw-r--r--   0        0        0      874 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/ontology.py
--rw-r--r--   0        0        0     8658 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-07-04 16:11:17.943206 encord-0.1.85/encord/orm/workflow.py
--rw-r--r--   0        0        0    41304 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-07-04 16:11:17.943206 encord-0.1.85/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    29244 2023-07-04 16:11:17.943206 encord-0.1.85/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-07-04 16:11:17.943206 encord-0.1.85/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1966 2023-07-04 16:11:17.943206 encord-0.1.85/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 encord-0.1.85/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-07-13 14:46:40.427879 encord-0.1.86/LICENSE
+-rw-r--r--   0        0        0     2030 2023-07-13 14:46:40.427879 encord-0.1.86/README.md
+-rw-r--r--   0        0        0      158 2023-07-13 14:46:40.447879 encord-0.1.86/encord/__init__.py
+-rw-r--r--   0        0        0      100 2023-07-13 14:46:40.447879 encord-0.1.86/encord/_version.py
+-rw-r--r--   0        0        0    49616 2023-07-13 14:46:40.447879 encord-0.1.86/encord/client.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/constants.py
+-rw-r--r--   0        0        0      508 2023-07-13 14:46:40.447879 encord-0.1.86/encord/common/enum.py
+-rw-r--r--   0        0        0    10852 2023-07-13 14:46:40.447879 encord-0.1.86/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/enums.py
+-rw-r--r--   0        0        0     3196 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/model.py
+-rw-r--r--   0        0        0     4522 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-07-13 14:46:40.447879 encord-0.1.86/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-07-13 14:46:40.447879 encord-0.1.86/encord/dataset.py
+-rw-r--r--   0        0        0     6355 2023-07-13 14:46:40.447879 encord-0.1.86/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/bundle.py
+-rw-r--r--   0        0        0      319 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/common.py
+-rw-r--r--   0        0        0      535 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/limits.py
+-rw-r--r--   0        0        0     7886 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/querier.py
+-rw-r--r--   0        0        0      747 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1738 2023-07-13 14:46:40.447879 encord-0.1.86/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/utils.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/__init__.py
+-rw-r--r--   0        0        0     3447 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/api_client.py
+-rw-r--r--   0        0        0      964 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/error_utils.py
+-rw-r--r--   0        0        0      216 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/payloads.py
+-rw-r--r--   0        0        0     2249 2023-07-13 14:46:40.451879 encord-0.1.86/encord/http/v2/request_signer.py
+-rw-r--r--   0        0        0      340 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/classification.py
+-rw-r--r--   0        0        0    21796 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/frames.py
+-rw-r--r--   0        0        0    22033 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   140628 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/project.py
+-rw-r--r--   0        0        0     1622 2023-07-13 14:46:40.451879 encord-0.1.86/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-07-13 14:46:40.451879 encord-0.1.86/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/analytics.py
+-rw-r--r--   0        0        0      982 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/api_key.py
+-rw-r--r--   0        0        0      486 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_interface.py
+-rw-r--r--   0        0        0     1418 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v1.py
+-rw-r--r--   0        0        0     1366 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v2.py
+-rw-r--r--   0        0        0     5335 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32989 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/dataset.py
+-rw-r--r--   0        0        0      829 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      256 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1241 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6667 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/model.py
+-rw-r--r--   0        0        0      874 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8658 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-07-13 14:46:40.451879 encord-0.1.86/encord/orm/workflow.py
+-rw-r--r--   0        0        0    41332 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-07-13 14:46:40.451879 encord-0.1.86/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29036 2023-07-13 14:46:40.451879 encord-0.1.86/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-07-13 14:46:40.451879 encord-0.1.86/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1989 2023-07-13 14:46:40.451879 encord-0.1.86/pyproject.toml
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 encord-0.1.86/PKG-INFO
```

### Comparing `encord-0.1.85/LICENSE` & `encord-0.1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/README.md` & `encord-0.1.86/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # The data engine for computer vision
 
 ## 💻 Features
 
 - Minimal low-level Python client that allows you to interact with Encord's API
-- Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11`
+- Supports Python: `3.8`, `3.9`, `3.10` and `3.11`
 
 ## ✨ Relevant Links
 
 * [Encord website](https://encord.com)
 * [Encord web app](https://app.encord.com)
 * [Encord documentation](https://docs.encord.com)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
 //opensource.org/licenses/Apache-2.0) # The data engine for computer vision ##
 ð» Features - Minimal low-level Python client that allows you to interact
-with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11` ##
-â¨ Relevant Links * [Encord website](https://encord.com) * [Encord web app]
-(https://app.encord.com) * [Encord documentation](https://docs.encord.com) ##
-ð¡ Getting Started For full documentation, please visit [Encord Python SDK]
-(https://python.docs.encord.com/). First, install Encord Python API Client
-using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
-```bash pip install encord ``` Then, generate an public-private key pair, and
-upload the public key to [Encord website](https://www.encord.com/). Detailed
-guide can be found in the [dedicated manual](https://docs.encord.com/admins/
-settings/public-keys/). Passing the private key to the factory, you can
-initialise the Encord client directly. ```python from encord import
-EncordUserClient user_client = EncordUserClient.create_with_ssh_private_key
-( "", password="", ) ``` Once you have instantiated an Encord client, it is
-easy to fetch a project information and start working with the platform. ```py
-project = user_client.get_project("") label_rows = project.list_label_rows_v2()
-``` For detailed examples and API reference please refer to [Encord SDK
-documentation](https://python.docs.encord.com/) ## ð Troubleshooting Please
-report bugs to the [GitHub Issues](https://github.com/encord-team/encord-
-client-python/issues). Just make sure you read the [Encord documentation]
-(https://docs.encord.com) and search for related issues first.
+with Encord's API - Supports Python: `3.8`, `3.9`, `3.10` and `3.11` ## â¨
+Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
+//app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
+Getting Started For full documentation, please visit [Encord Python SDK](https:
+//python.docs.encord.com/). First, install Encord Python API Client using the
+[pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
+install encord ``` Then, generate an public-private key pair, and upload the
+public key to [Encord website](https://www.encord.com/). Detailed guide can be
+found in the [dedicated manual](https://docs.encord.com/admins/settings/public-
+keys/). Passing the private key to the factory, you can initialise the Encord
+client directly. ```python from encord import EncordUserClient user_client =
+EncordUserClient.create_with_ssh_private_key( "", password="", ) ``` Once you
+have instantiated an Encord client, it is easy to fetch a project information
+and start working with the platform. ```py project = user_client.get_project
+("") label_rows = project.list_label_rows_v2() ``` For detailed examples and
+API reference please refer to [Encord SDK documentation](https://
+python.docs.encord.com/) ## ð Troubleshooting Please report bugs to the
+[GitHub Issues](https://github.com/encord-team/encord-client-python/issues).
+Just make sure you read the [Encord documentation](https://docs.encord.com) and
+search for related issues first.
```

### Comparing `encord-0.1.85/encord/client.py` & `encord-0.1.86/encord/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         """
         config = EncordConfig(resource_id, api_key, domain=domain, requests_settings=requests_settings)
         return EncordClientDataset.initialise_with_config(config, dataset_access_settings=dataset_access_settings)
 
     @staticmethod
     def initialise_with_config(
         config: ApiKeyConfig, dataset_access_settings: DatasetAccessSettings = DEFAULT_DATASET_ACCESS_SETTINGS
-    ) -> Union[EncordClientProject, EncordClientDataset]:
+    ) -> EncordClientDataset:
         """
         Create and initialize a Encord client from a Encord config instance.
 
         Args:
             config: A Encord config instance.
             dataset_access_settings: Set the dataset_access_settings if you would like to change the defaults.
 
@@ -367,26 +367,29 @@
             ResourceNotFoundError: If no dataset exists by the specified dataset EntityId.
             UnknownError: If an error occurs while retrieving the dataset.
         """
 
         created_before = parse_datetime("created_before", created_before)
         created_after = parse_datetime("created_after", created_after)
 
-        data_rows = self._querier.get_multiple(
-            DataRows,
-            payload={
-                "title_eq": title_eq,
-                "title_like": title_like,
-                "created_before": created_before,
-                "created_after": created_after,
-                "data_types": [data_type.to_upper_case_string() for data_type in data_types]
-                if data_types is not None
-                else None,
-                "dataset_access_settings": dataclasses.asdict(self._dataset_access_settings),
-            },
+        data_rows = cast(
+            List[DataRow],
+            self._querier.get_multiple(
+                DataRows,
+                payload={
+                    "title_eq": title_eq,
+                    "title_like": title_like,
+                    "created_before": created_before,
+                    "created_after": created_after,
+                    "data_types": [data_type.to_upper_case_string() for data_type in data_types]
+                    if data_types is not None
+                    else None,
+                    "dataset_access_settings": dataclasses.asdict(self._dataset_access_settings),
+                },
+            ),
         )
 
         for row in data_rows:
             row["_querier"] = self._querier
 
         return data_rows
```

### Comparing `encord-0.1.85/encord/configs.py` & `encord-0.1.86/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/constants/enums.py` & `encord-0.1.86/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/constants/model.py` & `encord-0.1.86/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/constants/model_weights.py` & `encord-0.1.86/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/constants/string_constants.py` & `encord-0.1.86/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/constants/test/test_enums.py` & `encord-0.1.86/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/dataset.py` & `encord-0.1.86/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/exceptions.py` & `encord-0.1.86/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/bundle.py` & `encord-0.1.86/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/constants.py` & `encord-0.1.86/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/error_utils.py` & `encord-0.1.86/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/querier.py` & `encord-0.1.86/encord/http/querier.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             raise ResourceNotFoundError(
                 f"[{object_type}] not found for query with uid=[{uid}] and payload=[{payload}]", context=context
             )
 
     @staticmethod
     def _parse_response(object_type: Type[T], item: dict) -> T:
         if issubclass(object_type, Formatter):
-            return object_type.from_dict(item)
+            return object_type.from_dict(item)  # type: ignore
         elif dataclasses.is_dataclass(object_type):
             return object_type(**item)  # type: ignore
         else:
             return object_type(item)  # type: ignore
 
     def basic_delete(self, db_object_type: Type[T], uid=None):
         """Single DB object getter."""
```

### Comparing `encord-0.1.85/encord/http/query_methods.py` & `encord-0.1.86/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/request.py` & `encord-0.1.86/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/utils.py` & `encord-0.1.86/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/v2/api_client.py` & `encord-0.1.86/encord/http/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/v2/error_utils.py` & `encord-0.1.86/encord/http/v2/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/http/v2/request_signer.py` & `encord-0.1.86/encord/http/v2/request_signer.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/bitmask.py` & `encord-0.1.86/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/common.py` & `encord-0.1.86/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/coordinates.py` & `encord-0.1.86/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/frames.py` & `encord-0.1.86/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/internal_helpers.py` & `encord-0.1.86/encord/objects/internal_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,15 @@
 
     elif isinstance(answer, Sequence):
         if len(answer) == 0:
             raise LabelRowError(
                 "Cannot infer the attribute if a list of answers is empty. Please provide the " "attribute explicitly."
             )
 
+        assert isinstance(answer[0], Option)  # Narrowing type here as sequence can contain only Options
         parent_opt = _search_for_parent(answer[0], attributes)
         if parent_opt is None:
             raise LabelRowError(
                 "Cannot find a corresponding attribute for one of the given answers in the Object ontology. "
                 "Please ensure to only pass the correct answer options for the given Object ontology. "
                 f"The used answer is `{answer}`"
             )
```

### Comparing `encord-0.1.85/encord/objects/ontology_labels_impl.py` & `encord-0.1.86/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1521,23 +1521,27 @@
         def frame(self) -> int:
             return self._frame
 
         @property
         def width(self) -> int:
             if self._label_row.data_type in [DataType.IMG_GROUP]:
                 return self._frame_level_data().width
-            else:
+            elif self._label_row_read_only_data.width is not None:
                 return self._label_row_read_only_data.width
+            else:
+                raise LabelRowError(f"Width is expected but not set for the data type {self._label_row.data_type}")
 
         @property
         def height(self) -> int:
             if self._label_row.data_type in [DataType.IMG_GROUP]:
                 return self._frame_level_data().height
-            else:
+            elif self._label_row_read_only_data.height is not None:
                 return self._label_row_read_only_data.height
+            else:
+                raise LabelRowError(f"Height is expected but not set for the data type {self._label_row.data_type}")
 
         @property
         def data_link(self) -> Optional[str]:
             if self._label_row.data_type not in [DataType.IMAGE, DataType.IMG_GROUP]:
                 raise LabelRowError("Data link can only be retrieved for DataType.IMAGE or DataType.IMG_GROUP")
             return self._frame_level_data().data_link
 
@@ -2763,21 +2767,21 @@
             self._set_answer_unsafe(answer_dict["answers"], attribute, track_hash, ranges)
         elif isinstance(attribute, RadioAttribute):
             if len(answer_dict["answers"]) == 1:
                 # When classification is removed in UI, it keeps the entry about the classification,
                 # but removes the answers.
                 # Thus an empty answers array is equivalent to "no such attribute", and such attribute should be ignored
                 feature_hash = answer_dict["answers"][0]["featureHash"]
-                option = _get_option_by_hash(feature_hash, attribute.options)
+                option = attribute.get_child_by_hash(feature_hash, type_=Option)
                 self._set_answer_unsafe(option, attribute, track_hash, ranges)
         elif isinstance(attribute, ChecklistAttribute):
             options = []
             for answer in answer_dict["answers"]:
                 feature_hash = answer["featureHash"]
-                option = _get_option_by_hash(feature_hash, attribute.options)
+                option = attribute.get_child_by_hash(feature_hash, type_=Option)
                 options.append(option)
             self._set_answer_unsafe(options, attribute, track_hash, ranges)
         else:
             raise NotImplementedError(f"The attribute type {type(attribute)} is not supported.")
 
     def _is_attribute_valid_child_of_object_instance(self, attribute: Attribute) -> bool:
         is_static_child = attribute.feature_node_hash in self._static_answer_map
```

### Comparing `encord-0.1.85/encord/objects/project.py` & `encord-0.1.86/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/objects/utils.py` & `encord-0.1.86/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/ontology.py` & `encord-0.1.86/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/analytics.py` & `encord-0.1.86/encord/orm/analytics.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/api_key.py` & `encord-0.1.86/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v1.py` & `encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/base_dto/base_dto_pydantic_v2.py` & `encord-0.1.86/encord/orm/base_dto/base_dto_pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/base_orm.py` & `encord-0.1.86/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/dataset.py` & `encord-0.1.86/encord/orm/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,20 +419,22 @@
             signed_url: If True, this will fetch a generated signed url of the data asset.
             images_data_fetch_options: If not None, this will fetch the image data of the data asset. You can
                 additionally specify what to fetch with the :class:`.ImagesDataFetchOptions` class.
             client_metadata: If True, this will fetch the client metadata of the data asset.
         """
         if self["_querier"] is not None:
             if images_data_fetch_options is not None:
-                images_data_fetch_options = dataclasses.asdict(images_data_fetch_options)
+                images_data_fetch_options_dict = dataclasses.asdict(images_data_fetch_options)
+            else:
+                images_data_fetch_options_dict = None
 
             payload = {
                 "additional_data": {
                     "signed_url": signed_url,
-                    "images_data_fetch_options": images_data_fetch_options,
+                    "images_data_fetch_options": images_data_fetch_options_dict,
                     "client_metadata": client_metadata,
                 }
             }
             res = self["_querier"].basic_getter(DataRow, uid=self.uid, payload=payload)
             self._update_current_class(res)
 
         else:
@@ -521,15 +523,15 @@
         super().__init__(
             {
                 "data_rows": data_rows,
             }
         )
 
     @classmethod
-    def from_dict(cls, json_dict: Dict) -> DataRow:
+    def from_dict(cls, json_dict: Dict) -> DataRow:  # type: ignore[override]
         return DataRow.from_dict(json_dict)
 
 
 @dataclasses.dataclass(frozen=True)
 class DatasetInfo:
     """
     This class represents a dataset in the context of listing
@@ -750,15 +752,15 @@
     Please update your SDK to the latest version. 
     """
 
     @staticmethod
     def from_str(string_location: str) -> StorageLocation:
         return STORAGE_LOCATION_BY_STR[string_location]
 
-    def get_str(self) -> str:
+    def get_str(self) -> str:  # type: ignore[return]
         if self == StorageLocation.CORD_STORAGE:
             return "CORD_STORAGE"
         elif self == StorageLocation.AWS:
             return "AWS_S3"
         elif self == StorageLocation.GCP:
             return "GCP_STR"
         elif self == StorageLocation.AZURE:
```

### Comparing `encord-0.1.85/encord/orm/dataset_with_user_role.py` & `encord-0.1.86/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/label_log.py` & `encord-0.1.86/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/label_row.py` & `encord-0.1.86/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/labeling_algorithm.py` & `encord-0.1.86/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/model.py` & `encord-0.1.86/encord/orm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 @dataclass
 class TrainingMetadata(Formatter):
     model_iteration_uid: str
     created_at: Optional[datetime] = None
     training_final_loss: Optional[float] = None
-    model_training_labels: Optional[List[ModelTrainingLabel]] = None
+    model_training_labels: Optional[ModelTrainingLabel] = None
 
     @classmethod
     def from_dict(cls, json_dict: dict):
         return TrainingMetadata(
             model_iteration_uid=json_dict["model_iteration_uid"],
             created_at=cls.get_created_at(json_dict),
             training_final_loss=json_dict["training_final_loss"],
@@ -137,15 +137,15 @@
         created_at = json_dict["created_at"]
         if created_at is None:
             return None
 
         return parse(created_at)
 
     @staticmethod
-    def get_model_training_labels(json_dict: dict) -> Optional[List[ModelTrainingLabel]]:
+    def get_model_training_labels(json_dict: dict) -> Optional[ModelTrainingLabel]:
         model_training_labels = json_dict["model_training_labels"]
         if model_training_labels is None:
             return None
 
         return ModelTrainingLabel.from_dict(model_training_labels)
```

### Comparing `encord-0.1.85/encord/orm/ontology.py` & `encord-0.1.86/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/project.py` & `encord-0.1.86/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/project_api_key.py` & `encord-0.1.86/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/project_with_user_role.py` & `encord-0.1.86/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/orm/test/test_dataset.py` & `encord-0.1.86/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/project.py` & `encord-0.1.86/encord/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,16 @@
             data_title_eq=data_title_eq,
             data_title_like=data_title_like,
             workflow_graph_node_title_eq=workflow_graph_node_title_eq,
             workflow_graph_node_title_like=workflow_graph_node_title_like,
         )
 
         label_rows = [
-            LabelRowV2(label_row_metadata, self._client, self._ontology) for label_row_metadata in label_row_metadatas
+            LabelRowV2(label_row_metadata, self._client, self._ontology)  # type: ignore
+            for label_row_metadata in label_row_metadatas
         ]
         return label_rows
 
     def add_users(self, user_emails: List[str], user_role: ProjectUserRole) -> List[ProjectUser]:
         """
         Add users to project
```

### Comparing `encord-0.1.85/encord/project_ontology/classification_attribute.py` & `encord-0.1.86/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/project_ontology/classification_option.py` & `encord-0.1.86/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/project_ontology/ontology.py` & `encord-0.1.86/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/project_ontology/ontology_classification.py` & `encord-0.1.86/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/project_ontology/ontology_object.py` & `encord-0.1.86/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/user_client.py` & `encord-0.1.86/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from dateutil import parser as datetime_parser
 
-# add this for backward compatible class comparisons
-# pylint: disable-next=import-error
-from cord.utilities.client_utilities import (
-    LocalImport as CordLocalImport,  # type: ignore
-)
 from encord.client import EncordClient, EncordClientDataset, EncordClientProject
 from encord.configs import SshConfig, UserConfig, get_env_ssh_key
 from encord.constants.string_constants import TYPE_DATASET, TYPE_ONTOLOGY, TYPE_PROJECT
 from encord.dataset import Dataset
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
@@ -404,15 +399,15 @@
             CvatImporterSuccess: If the project was successfully imported.
             CvatImporterError: If the project could not be imported.
 
         Raises:
             ValueError:
                 If the CVAT directory has an invalid format.
         """
-        if not isinstance(import_method, (LocalImport, CordLocalImport)):
+        if not isinstance(import_method, LocalImport):
             raise ValueError("Only local imports are currently supported ")
 
         cvat_directory_path = import_method.file_path
 
         directory_path = Path(cvat_directory_path)
         images_directory_path = directory_path.joinpath("images")
         if images_directory_path not in list(directory_path.iterdir()):
```

### Comparing `encord-0.1.85/encord/utilities/client_utilities.py` & `encord-0.1.86/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/utilities/label_utilities.py` & `encord-0.1.86/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/encord/utilities/project_user.py` & `encord-0.1.86/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.85/pyproject.toml` & `encord-0.1.86/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.85"
+version = "0.1.86"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
-keywords = ["cord", "encord"]
+keywords = ["encord"]
 packages = [
-    { include = "cord"},
     { include = "encord"},
 ]
 readme = "README.md"
 repository="https://github.com/encord-team/encord-client-python"
 documentation="https://python.docs.encord.com/"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 python-dateutil = "^2.8.2"
 requests = "^2.25.0"
 cryptography = ">=3.4.8"
 tqdm = "^4.32.1"
-importlib_metadata = {version = "^6.1.0", python = "<3.8"}
 pydantic = ">=1.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
-pre-commit = "^2.16.0"
+pre-commit = "^3.3.0"
 black = "^23.3.0"
 sphinx-tabs = "^3.3.1"
 sphinx-autodoc-typehints = "1.15.2"
 sphinx-codeautolink = "^0.10.0"
 sphinx-copybutton = "^0.5.0"
 sphinx-toolbox = "^3.4.0"
 prettyprinter = "0.18.0"
@@ -41,14 +39,17 @@
 pydata-sphinx-theme = "^0.8.1"
 Pillow = "^9.1.0"
 sphinx-gallery = "^0.10.1"
 deepdiff = "^6.2.1"
 types-requests = "^2.25.0"
 pylint = "^2.13.9"
 autoflake = "^2.1.1"
+mypy = "^1.4.1"
+types-python-dateutil = "^2.8.19"
+types-tqdm = "^4.32.1"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -72,7 +73,10 @@
 expand-star-imports = true
 ignore-init-module-imports = true
 in-place = true
 recursive = true
 remove-all-unused-imports = true
 remove-duplicate-keys = true
 remove-unused-variables = true
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `encord-0.1.85/PKG-INFO` & `encord-0.1.86/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.85
+Version: 0.1.86
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
-Keywords: cord,encord
+Keywords: encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=3.4.8)
-Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0) ; python_version < "3.8"
 Requires-Dist: pydantic (>=1.7.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: tqdm (>=4.32.1,<5.0.0)
 Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
 Description-Content-Type: text/markdown
@@ -37,15 +35,15 @@
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # The data engine for computer vision
 
 ## 💻 Features
 
 - Minimal low-level Python client that allows you to interact with Encord's API
-- Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11`
+- Supports Python: `3.8`, `3.9`, `3.10` and `3.11`
 
 ## ✨ Relevant Links
 
 * [Encord website](https://encord.com)
 * [Encord web app](https://app.encord.com)
 * [Encord documentation](https://docs.encord.com)
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.85 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.86 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
-Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
-Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
+Apache Software License Keywords: encord Author: Cord Technologies Limited
+Author-email: hello@encord.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: cryptography (>=3.4.8) Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0)
-; python_version < "3.8" Requires-Dist: pydantic (>=1.7.0) Requires-Dist:
-python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0)
-Requires-Dist: tqdm (>=4.32.1,<5.0.0) Project-URL: Documentation, https://
-python.docs.encord.com/ Project-URL: Repository, https://github.com/encord-
-team/encord-client-python Description-Content-Type: text/markdown
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: cryptography (>=3.4.8) Requires-Dist: pydantic
+(>=1.7.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist:
+requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm (>=4.32.1,<5.0.0) Project-URL:
+Documentation, https://python.docs.encord.com/ Project-URL: Repository, https:/
+/github.com/encord-team/encord-client-python Description-Content-Type: text/
+markdown
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
 //opensource.org/licenses/Apache-2.0) # The data engine for computer vision ##
 ð» Features - Minimal low-level Python client that allows you to interact
-with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11` ##
-â¨ Relevant Links * [Encord website](https://encord.com) * [Encord web app]
-(https://app.encord.com) * [Encord documentation](https://docs.encord.com) ##
-ð¡ Getting Started For full documentation, please visit [Encord Python SDK]
-(https://python.docs.encord.com/). First, install Encord Python API Client
-using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
-```bash pip install encord ``` Then, generate an public-private key pair, and
-upload the public key to [Encord website](https://www.encord.com/). Detailed
-guide can be found in the [dedicated manual](https://docs.encord.com/admins/
-settings/public-keys/). Passing the private key to the factory, you can
-initialise the Encord client directly. ```python from encord import
-EncordUserClient user_client = EncordUserClient.create_with_ssh_private_key
-( "", password="", ) ``` Once you have instantiated an Encord client, it is
-easy to fetch a project information and start working with the platform. ```py
-project = user_client.get_project("") label_rows = project.list_label_rows_v2()
-``` For detailed examples and API reference please refer to [Encord SDK
-documentation](https://python.docs.encord.com/) ## ð Troubleshooting Please
-report bugs to the [GitHub Issues](https://github.com/encord-team/encord-
-client-python/issues). Just make sure you read the [Encord documentation]
-(https://docs.encord.com) and search for related issues first.
+with Encord's API - Supports Python: `3.8`, `3.9`, `3.10` and `3.11` ## â¨
+Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
+//app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
+Getting Started For full documentation, please visit [Encord Python SDK](https:
+//python.docs.encord.com/). First, install Encord Python API Client using the
+[pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
+install encord ``` Then, generate an public-private key pair, and upload the
+public key to [Encord website](https://www.encord.com/). Detailed guide can be
+found in the [dedicated manual](https://docs.encord.com/admins/settings/public-
+keys/). Passing the private key to the factory, you can initialise the Encord
+client directly. ```python from encord import EncordUserClient user_client =
+EncordUserClient.create_with_ssh_private_key( "", password="", ) ``` Once you
+have instantiated an Encord client, it is easy to fetch a project information
+and start working with the platform. ```py project = user_client.get_project
+("") label_rows = project.list_label_rows_v2() ``` For detailed examples and
+API reference please refer to [Encord SDK documentation](https://
+python.docs.encord.com/) ## ð Troubleshooting Please report bugs to the
+[GitHub Issues](https://github.com/encord-team/encord-client-python/issues).
+Just make sure you read the [Encord documentation](https://docs.encord.com) and
+search for related issues first.
```

