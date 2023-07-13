# Comparing `tmp/arthurai-3.8.8.tar.gz` & `tmp/arthurai-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthurai-3.8.8.tar", last modified: Wed May 12 14:51:53 2021, max compression
+gzip compressed data, was "arthurai-3.9.0.tar", last modified: Tue Jun 15 13:32:19 2021, max compression
```

## Comparing `arthurai-3.8.8.tar` & `arthurai-3.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/
--rw-rw-rw-   0 root         (0) root         (0)       41 2021-05-12 14:51:43.000000 arthurai-3.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      628 2021-05-12 14:51:53.000000 arthurai-3.8.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/
--rw-rw-rw-   0 root         (0) root         (0)      256 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/client/
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/client/apiv3/
--rw-rw-rw-   0 root         (0) root         (0)     1722 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/client/apiv3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     6940 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/client/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2948 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/common/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/common/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/base.py
--rw-rw-rw-   0 root         (0) root         (0)    11391 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/data_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    97948 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5482 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/core/viz/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/viz/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/viz/style.py
--rw-rw-rw-   0 root         (0) root         (0)     1126 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/viz/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13755 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/core/viz/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai/explainability/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/explainability/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27364 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/explainability/arthur_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    19877 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/explainability/explanation_packager.py
--rw-rw-rw-   0 root         (0) root         (0)     5055 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/util.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2021-05-12 14:51:43.000000 arthurai-3.8.8/arthurai/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      628 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1565 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      340 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-05-12 14:51:53.000000 arthurai-3.8.8/arthurai.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2021-05-12 14:51:53.000000 arthurai-3.8.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1412 2021-05-12 14:51:43.000000 arthurai-3.8.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      264 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/base_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4081 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_alert_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_arthur_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     9601 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_core_util.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_data_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_explanation_packager.py
--rw-rw-rw-   0 root         (0) root         (0)     5492 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_file_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     5820 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_inferences.py
--rw-rw-rw-   0 root         (0) root         (0)     6937 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_model_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    11430 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1342 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_models_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_reference_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-12 14:51:53.000000 arthurai-3.8.8/tests/test_request_models/
--rw-rw-rw-   0 root         (0) root         (0)      218 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_request_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17182 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_request_models/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_request_models/test_alert_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_request_models/test_attribute_category.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2021-05-12 14:51:43.000000 arthurai-3.8.8/tests/test_request_models/test_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2021-06-15 13:32:07.000000 arthurai-3.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      617 2021-06-15 13:32:19.000000 arthurai-3.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/
+-rw-rw-rw-   0 root         (0) root         (0)      256 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/client/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/client/apiv3/
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/client/apiv3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11847 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6940 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/client/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/common/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/common/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11391 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/data_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)   102317 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/core/viz/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/viz/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/viz/style.py
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/viz/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13755 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/core/viz/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai/explainability/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/explainability/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26994 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/explainability/arthur_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19877 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/explainability/explanation_packager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2021-06-15 13:32:07.000000 arthurai-3.9.0/arthurai/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      617 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1565 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      340 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-06-15 13:32:19.000000 arthurai-3.9.0/arthurai.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2021-06-15 13:32:19.000000 arthurai-3.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2021-06-15 13:32:07.000000 arthurai-3.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/base_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_alert_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_arthur_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    10435 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_core_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     5273 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_data_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_explanation_packager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_file_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5820 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_inferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     6937 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_model_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    12966 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_models_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_reference_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-15 13:32:19.000000 arthurai-3.9.0/tests/test_request_models/
+-rw-rw-rw-   0 root         (0) root         (0)      218 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_request_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17182 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_request_models/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_request_models/test_alert_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_request_models/test_attribute_category.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2021-06-15 13:32:07.000000 arthurai-3.9.0/tests/test_request_models/test_model.py
```

### Comparing `arthurai-3.8.8/PKG-INFO` & `arthurai-3.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: arthurai
-Version: 3.8.8
+Version: 3.9.0
 Summary: Python SDK for ArthurAI
 Home-page: https://arthur.ai
 Author: ArthurAI
 Author-email: info@arthur.ai
 License: MIT
-Description: UNKNOWN
 Keywords: api arthur ArthurAI sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+
+UNKNOWN
+
```

### Comparing `arthurai-3.8.8/arthurai/client/apiv3/__init__.py` & `arthurai-3.9.0/arthurai/client/apiv3/__init__.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/client/base.py` & `arthurai-3.9.0/arthurai/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import platform
 import requests
 import concurrent.futures
 import threading
 import time
 import logging
 from urllib.parse import urlparse
+from http import HTTPStatus
 
 from typing import Optional
 
-from arthurai.common.exceptions import MissingParameterError, InternalValueError
+from arthurai.client.validation import validate_response_status
+from arthurai.common.exceptions import MissingParameterError, InternalValueError, UserValueError
 from arthurai.version import __version__
 
 logger = logging.getLogger(__name__)
 
 
 class BaseApiClient(object):
     """docstring for BaseApiClient"""
@@ -62,22 +64,23 @@
             user_org = self._get_current_user_org()
             agent_info = f"arthur-sdk/{__version__} (system={platform.system()}, org={user_org})" if user_org \
                 else f"arthur-sdk/{__version__} (system={platform.system()})"
             self.user_agent = agent_info
 
     def _get_current_user_org(self) -> Optional[str]:
         url = f"{self.base_path}/users/me"
-        resp = self.get(url, return_raw_response=True)
-        if resp.status_code == 200:
-            response_body = resp.json()
-            if "organization_id" in response_body:
-                return response_body["organization_id"]
-        else:
-            logger.debug(f"Failed to get current user organization, received response code {resp.status_code} with body {resp.content}")
-        return None
+        try:
+            resp = self.get(url, return_raw_response=True)
+        except requests.RequestException as e:
+            raise UserValueError(f"Failed to connect to {self.url}, please ensure the URL is correct") from e
+        if resp.status_code == HTTPStatus.UNAUTHORIZED:
+            raise UserValueError(f"Unauthorized, please ensure your access key is correct")
+        validate_response_status(resp, HTTPStatus.OK)
+        response_body = resp.json()
+        return response_body.get("organization_id", None)
 
     def send(self, url, method='GET', data=None, files=None, params=None, headers=None, return_raw_response=False,
              retries=0):
         """Sends the specified data with headers to the given url with the given request type
 
         :param retries: Number of times to retry the request if it results in a 400 or higher response code
         :param return_raw_response: If true do not filter request response, return raw object
```

### Comparing `arthurai-3.8.8/arthurai/client/client.py` & `arthurai-3.9.0/arthurai/client/client.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/client/validation.py` & `arthurai-3.9.0/arthurai/client/validation.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/common/constants.py` & `arthurai-3.9.0/arthurai/common/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,26 @@
     NLP = "NLP"
 
 
 class OutputType(ListableStrEnum):
     Regression = "REGRESSION"
     Multiclass = "MULTICLASS"
     Multilabel = "MULTILABEL"
+    ObjectDetection = "OBJECT_DETECTION"
 
 
 class ValueType(ListableStrEnum):
     String = "STRING"
     Integer = "INTEGER"
     Float = "FLOAT"
     Image = "IMAGE"
     Boolean = "BOOLEAN"
     Timestamp = "TIMESTAMP"
-    Unstructured_Text = "UNSTRUCTURED_TEXT"
+    Unstructured_Text = "UNSTRUCTURED_TEXT" # don't remove old one, backward compatibility
+    BoundingBox = "BOUNDING_BOX"
 
 
 class Stage(ListableStrEnum):
     ModelPipelineInput = "PIPELINE_INPUT"
     PredictFunctionInput = "PREDICT_FUNCTION_INPUT"
     PredictedValue = "PREDICTED_VALUE"
     NonInputData = "NON_INPUT_DATA"
```

### Comparing `arthurai-3.8.8/arthurai/common/exceptions.py` & `arthurai-3.9.0/arthurai/common/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 
 import functools
+import inspect
+
 
 # Base Error
 class ArthurError(Exception):
     """
     Base Error for Arthur SDK. This class should not be used directly, Arthur exceptions should inherit from either
     ArthurUserError or ArthurInternalError.
     """
@@ -109,14 +111,27 @@
         prefix = ""
     else:
         prefix = message + " because "
 
     def decorator_arthur_excepted(func):
         @functools.wraps(func)
         def wrapper_arthur_excepted(*args, **kwargs):
+            # ensure all required parameters are present: check manually because TypeErrors from internal calls
+            #  should not be UserErrors
+            try:
+                inspect.signature(func).bind(*args, **kwargs)
+                success = True
+                err_msg = None
+            except TypeError as e:
+                success = False
+                err_msg = str(e)
+            if not success:
+                raise MissingParameterError(err_msg)
+
+            # call the function
             try:
                 return func(*args, **kwargs)
             # if it is a user error simply re-raise
             except ArthurUserError as e:
                 raise e
             # otherwise wrap it in a message saying it's not the user's fault
             except ArthurInternalError as e:
@@ -124,9 +139,9 @@
             except Exception as e:
                 raise ArthurInternalError(prefix +
                                           "there was an unexpected internal exception, please report to Arthur") from e
         return wrapper_arthur_excepted
     return decorator_arthur_excepted
 
 
-
-# TODO: TU-96 can we add custom linting steps to check that base exceptions aren't raised/caught and only arthur exceptions are used?
+# TODO: TU-96 can we add custom linting steps to check that base exceptions aren't raised/caught and only arthur
+#  exceptions are used?
```

### Comparing `arthurai-3.8.8/arthurai/common/log.py` & `arthurai-3.9.0/arthurai/common/log.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/alerts.py` & `arthurai-3.9.0/arthurai/core/alerts.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/attributes.py` & `arthurai-3.9.0/arthurai/core/attributes.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/base.py` & `arthurai-3.9.0/arthurai/core/base.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/data_service.py` & `arthurai-3.9.0/arthurai/core/data_service.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/decorators.py` & `arthurai-3.9.0/arthurai/core/decorators.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/models.py` & `arthurai-3.9.0/arthurai/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     attributes: Optional[List[ArthurAttribute]] = None
     tags: Optional[List[str]] = None
     classifier_threshold: Optional[float] = None
     text_delimiter: Optional[TextDelimiter] = None
     expected_throughput_gb_per_day: Optional[int] = None
     pixel_height: Optional[int] = None
     pixel_width: Optional[int] = None
+    image_class_labels: Optional[List[str]] = None
 
     def __post_init__(self, client: BaseApiClient):
         # variables created here will only be accessible directly on the object itself, they will not be in the result
         # of object.to_dict() even if marked as public (does not have preceding underscore)
         self._client = client
         self._explainer: Optional[ExplanationPackager] = None
         self.viz = DataVisualizer(self)
@@ -240,47 +241,60 @@
             categorical = False
         elif value_type == ValueType.Integer and cnt_distinct <= 20:
             categorical = True
         elif value_type == ValueType.Integer:
             categorical = False
         elif value_type == ValueType.Unstructured_Text:
             categorical = True
+        elif value_type == ValueType.Image:
+            categorical = False
         else:
             categorical = True
 
         # even if unstructured text attributes aren't unique, we don't want categories
         if categorical and not attribute_data["is_unique"] and not value_type == ValueType.Unstructured_Text:
             attribute_data["categories"] = [AttributeCategory(value=str(cat)) for cat in
                                             list(set(attribute_data_series))]
-        elif not categorical:
+        # if not categorical, and numerical, set min/max
+        elif not categorical and value_type in [ValueType.Float, ValueType.Integer, ValueType.Boolean]:
             attribute_data["min_range"] = core_util.NumpyEncoder.convert_value(attribute_data_series.min())
             attribute_data["max_range"] = core_util.NumpyEncoder.convert_value(attribute_data_series.max())
 
         attribute_data["categorical"] = categorical
 
         return attribute_data
 
-    @staticmethod
-    def _to_arthur_dtype(dtype: str) -> ValueType:
+    def _to_arthur_dtype(self, dtype: str, series: Series) -> ValueType:
         """Select an :py:class:`.DataType` based on a pandas dtype
 
         :param dtype: the pandas dtype
+        :param example_val: an example value, used to confirm 'object' is actually string
         :return: The :py:class:`.DataType` corresponding to the pandas dtype
         """
 
-        if dtype in ["string", "object"]:
-            return ValueType.String
+        # in case of someone sending all nulls in a column, you can end up with empty series
+        # handle example val of none, will not be able to distinguish between string or list, but should be edge case
+        # and passing lists isn't expected, but we should handle most cases
+        example_val = series[0] if len(series) > 0 else None
+
+        if dtype in ["string", "object"] and (isinstance(example_val, str) or example_val is None):
+            if self.input_type == InputType.Image:
+                return ValueType.Image
+            else:
+                return ValueType.String
         elif dtype in ["bool", "boolean"]:
             return ValueType.Boolean
         elif re.search("u?int*", dtype, flags=re.I) or re.search("u?Int*", dtype, flags=re.I):
             return ValueType.Integer
         elif re.search("float*", dtype, flags=re.I):
             return ValueType.Float
         elif re.search("(datetime|timestamp).*", dtype, flags=re.I):
             return ValueType.Timestamp
+        else:
+            return None
 
     @arthur_excepted("failed to parse dataframe")
     def from_dataframe(self, data: Union[DataFrame, Series], stage: Stage) -> None:
         """ Attempt to autogenerate attributes based on input data.
 
         Note that this does *not* automatically set reference
         data; this method only reads the passed-in data, and then infers attribute names, types, etc. and sets them up
@@ -294,42 +308,51 @@
         :raise: ArthurUserError: failed due to user error
         :raise: ArthurInternalError: failed due to an internal error
         """
 
         if stage == Stage.PredictedValue or stage == Stage.GroundTruth:
             raise MethodNotApplicableError("Use either add_regression_output_attributes(), "
                                            "add_multiclass_classifier_output_attributes(), "
-                                           "or add_binary_classifier_output_attributes() to add output attributes.")
+                                           "add_binary_classifier_output_attributes(), "
+                                           "or add_object_detection_output_attributes() to add output attributes.")
 
         if isinstance(data, DataFrame):
             df = data
         elif isinstance(data, Series):
             df = data.to_frame()
         else:
             raise UserTypeError("Unsupported data type: a pandas.DataFrame or pandas.Series is required")
 
+        if len(df) == 0:
+            raise UserValueError("Dataframe must have at least 1 row of data")
+
         found_categorical = False
         for idx, column in enumerate(df.columns):
 
             series = core_util.standardize_pd_obj(df[column], dropna=True, replacedatetime=False,
                                                   attributes=self.attributes_type_dict)
-            value_type = self._to_arthur_dtype(series.dtype.name)
+            value_type = self._to_arthur_dtype(series.dtype.name, series)
+            # handle unknown datatype
+            if value_type is None:
+                logger.warning(f"Cannot parse type {series.dtype.name} for column {column}. Not including in schema. "
+                                f"Valid types are: str, int, float, datetime, timestamp, bool. "
+                                "To manually add an attribute use model.add_attribute(). Run help(model.add_attribute) for full documentation.")
+                continue
 
             try:
                 attribute_data = self._get_attribute_data(value_type, series)
             except ArthurUserError as e:
                 raise ArthurUserError(f"Error in column: {column}: {str(e)}")
 
             if value_type == ValueType.String and self.input_type == InputType.NLP:
                 value_type = ValueType.Unstructured_Text
                 # even if unstructured text attributes are not unique we don't want to store categories
                 attribute_data['categories'] = None
 
-            if value_type == ValueType.String and self.input_type == InputType.Image:
-                value_type = ValueType.Image
+            if value_type == ValueType.Image:
                 # even if image attributes are not unique we don't want to store categories
                 attribute_data['categories'] = None
             
             if attribute_data['categorical'] and value_type != ValueType.Unstructured_Text:
                 found_categorical = True
                 
 
@@ -683,14 +706,64 @@
             self._add_attribute_to_model(arthur_gt_attr)
             self._add_attribute_to_model(arthur_pred_attr)
             attributes_added[arthur_pred_attr.name] = arthur_pred_attr
             attributes_added[arthur_gt_attr.name] = arthur_gt_attr
         self.classifier_threshold = threshold
         return attributes_added
 
+    @arthur_excepted("failed to add output attributes")
+    def add_object_detection_output_attributes(self, predicted_attr_name: str,
+                                                gt_attr_name: str,
+                                                image_class_labels: List[str]) -> Dict[str, ArthurAttribute]:
+        """Registers ground truth and predicted value attributes for an object detection model, as well as
+        setting the image class labels.
+
+        This function will create a predicted value attribute and ground truth attribute using the names provided,
+        giving each a value type of Bounding Box. Image class labels are also set on the model object. The index
+        of each label in the list should correspond to a class_id the model outputs.
+
+        Ex: image_class_labels = ['cat', 'dog', 'person']
+        So a bounding box with class_id of 0 would have label 'cat', class_id of 2 would have label 'person'
+
+        :param predicted_attr_name: The name of the predicted value attribute
+        :param gt_attr_name: The name of the ground truth attribute
+        :param image_class_labels: The labels for each class the model can predict, ordered by their class_id
+        
+        :return: Mapping of added attributes string name -> ArthurAttribute Object
+        :raise: ArthurUserError: failed due to user error
+        :raise: ArthurInternalError: failed due to an internal error
+        """
+        if predicted_attr_name == gt_attr_name:
+            raise UserValueError("Predicted value attribute name matched ground truth attribute name. Attribute names must be unique")
+        if len(image_class_labels) == 0:
+            raise UserValueError("Must provide at least one class label")
+        if self.input_type != InputType.Image or self.output_type != OutputType.ObjectDetection:
+            raise MethodNotApplicableError("This function can only be called for models with Image input and Object Detection output")
+
+        arthur_gt_attr = ArthurAttribute(
+            name=gt_attr_name,
+            stage=Stage.GroundTruth,
+            value_type=ValueType.BoundingBox,
+            attribute_link=predicted_attr_name,
+            position=0
+        )
+        arthur_pred_attr = ArthurAttribute(
+            name=predicted_attr_name,
+            stage=Stage.PredictedValue,
+            value_type=ValueType.BoundingBox,
+            attribute_link=gt_attr_name,
+            position=0
+        )
+        self._add_attribute_to_model(arthur_gt_attr)
+        self._add_attribute_to_model(arthur_pred_attr)
+        self.image_class_labels = image_class_labels
+
+        return {predicted_attr_name: arthur_pred_attr, gt_attr_name: arthur_gt_attr}
+        
+
     @arthur_excepted("failed to get attribute")
     def get_attribute(self, name: str, stage: Optional[Stage] = None) -> ArthurAttribute:
         """Retrieves an attribute by name and stage
 
         :param name: string name of the attribute to retrieve
         :param stage: Optional `Stage` of attribute to retrieve
 
@@ -899,14 +972,16 @@
         :raise: ArthurUserError: failed due to user error
         :raise: ArthurInternalError: failed due to an internal error
         """
         if self.input_type == InputType.NLP and self.text_delimiter is None:
             raise MissingParameterError("Must set a text delimiter for NLP models prior to enabling explainability")
         if python_version is None:
             python_version = f'{sys.version_info[0]}.{sys.version_info[1]}'
+            if sys.version_info[0] == 3 and sys.version_info[1] >= 9:
+                raise UserValueError("Explainability not supported for Python 3.9 and greater. Please use Python 3.8")
         if self.input_type != InputType.Image and df is None:
             raise MissingParameterError("Must provide example dataframe for NLP and Tabular models")
         if project_directory is None:
             raise MissingParameterError("project_directory must be specified")
         if user_predict_function_import_path is None:
             raise MissingParameterError("user_predict_function_import_path must be specified")
         if df is not None and len(df) < 5000:
```

### Comparing `arthurai-3.8.8/arthurai/core/util.py` & `arthurai-3.9.0/arthurai/core/util.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/viz/utils.py` & `arthurai-3.9.0/arthurai/core/viz/utils.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/core/viz/visualizer.py` & `arthurai-3.9.0/arthurai/core/viz/visualizer.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/explainability/arthur_explainer.py` & `arthurai-3.9.0/arthurai/explainability/arthur_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,26 +79,22 @@
         self.tabular_explainer_lime = None
 
         # build tabular explainers
         if self.model_input_type == InputType.Tabular:
             self.build_tabular_explainers(enable_lime=self.enable_lime, enable_shap=self.enable_shap, data=encoded_data)
         if self.model_input_type == InputType.NLP:
             if self.enable_shap:
-                logger.warning("`enable_shap` was set to True, but SHAP is currently not supported for NLP models. "
-                               "Automatically disabling SHAP")
                 self.enable_shap = False
             # currently only Lime is supported for NLP, hardcode in args for now
             self.enable_lime = True
             self.build_nlp_explainers(enable_lime=self.enable_lime, enable_shap=self.enable_shap, data=encoded_data)
         if self.model_input_type == InputType.Image:
             if self.load_image_func is None:
                 raise UserValueError('load_image_func must be provided for image explanations')
             if self.enable_shap:
-                logger.warning("`enable_shap` was set to True, but SHAP is currently not supported for CV/ImageInput models. "
-                               "Automatically disabling SHAP")
                 self.enable_shap = False
             # currently only Lime is supported for CV/ImageInput, hardcode in args for now
             self.enable_lime = True
             self.build_image_explainers(enable_lime=self.enable_lime, enable_shap=self.enable_shap, data=encoded_data)
         # not supported input type
         else:
             pass
```

### Comparing `arthurai-3.8.8/arthurai/explainability/explanation_packager.py` & `arthurai-3.9.0/arthurai/explainability/explanation_packager.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai/util.py` & `arthurai-3.9.0/arthurai/util.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/arthurai.egg-info/PKG-INFO` & `arthurai-3.9.0/arthurai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: arthurai
-Version: 3.8.8
+Version: 3.9.0
 Summary: Python SDK for ArthurAI
 Home-page: https://arthur.ai
 Author: ArthurAI
 Author-email: info@arthur.ai
 License: MIT
-Description: UNKNOWN
 Keywords: api arthur ArthurAI sdk
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+
+UNKNOWN
+
```

### Comparing `arthurai-3.8.8/arthurai.egg-info/SOURCES.txt` & `arthurai-3.9.0/arthurai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/setup.py` & `arthurai-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/base_test.py` & `arthurai-3.9.0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/conftest.py` & `arthurai-3.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_alert_rule.py` & `arthurai-3.9.0/tests/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_arthur_explainer.py` & `arthurai-3.9.0/tests/test_arthur_explainer.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_client.py` & `arthurai-3.9.0/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 
 from tests import MockResponse
 
 from arthurai import ArthurAI
 from arthurai.common.constants import InputType, OutputType
 from arthurai.client.validation import validate_multistatus_response_and_get_failures, validate_response_status
 from arthurai.common.exceptions import ResponseServerError, ResponseClientError, ResponseRedirectError, \
-    InternalValueError
+    InternalValueError, UserValueError
 from tests.base_test import BaseTest
 
 
 class TestClient(BaseTest):
 
     def _mock_get_user(self):
-        self.mockPost(f"/api/v3/users/me", request_type=responses.GET, status=200,
+        self.mockPost(f"/api/v3/users/me", request_type=responses.GET, status=HTTPStatus.OK,
                       dict_to_return={"organization_id": "65624ee6-9a73-4fe3-a7ff-8612f7d11c21", "role": "Model Owner"})
 
+    def _mock_get_user_unauthorized(self):
+        self.mockPost(f"/api/v3/users/me", request_type=responses.GET, status=HTTPStatus.UNAUTHORIZED,
+                      dict_to_return={"bad": "user"})
+
     @pytest.mark.usefixtures('mock_cred_env_vars')
     def test_client_init_env_vars(self):
         client = ArthurAI(offline=True)
         assert client.client.url == 'http://mock'
         assert client.client.access_key == 'access_key'
 
         client = ArthurAI(url="this is a url", access_key="this is an access key", offline=True)
@@ -59,14 +63,27 @@
 
         ArthurAI(access_key=self.access_key, url=self._base_url)
         self.assertEqual(len(responses.calls), 1)
         expectedResponse = {'organization_id': '65624ee6-9a73-4fe3-a7ff-8612f7d11c21', 'role': 'Model Owner'}
         self.assertEqual(expectedResponse, responses.calls[0].response.json())
 
     @responses.activate
+    def test_client_init_bad_host(self):
+        with pytest.raises(UserValueError, match=".*please ensure the URL is correct.*"):
+            ArthurAI(access_key=self.access_key, url=self._base_url)
+        self.assertEqual(len(responses.calls), 1)
+
+    @responses.activate
+    def test_client_init_bad_access_key(self):
+        self._mock_get_user_unauthorized()
+        with pytest.raises(UserValueError, match=".*please ensure your access key is correct.*"):
+            ArthurAI(access_key=self.access_key, url=self._base_url)
+        self.assertEqual(len(responses.calls), 1)
+
+    @responses.activate
     def test_client_init_offline(self):
         ArthurAI(access_key=self.access_key, url=self._base_url, offline=True)
         self.assertEqual(len(responses.calls), 0)
 
     @responses.activate
     def test_client_init_offlines(self):
         self.mockPost(f"/api/v3/models/1234", request_type=responses.GET, status=200,
```

### Comparing `arthurai-3.8.8/tests/test_data_service.py` & `arthurai-3.9.0/tests/test_data_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def test_chunk_parquet_image_set_single_file():
     # create test parquet set
     image_dir = pathlib.Path(__file__).parent.absolute()
     image_path = os.path.join(image_dir, "data", "test_image.png")
 
     # we want to generate 400 MB of image data, to ensure we get 2 chunks
-    target_size = 400000000 # 400 MB in bytes
+    target_size = 400000000  # 400 MB in bytes
     image_size = os.path.getsize(image_path)
     num_images = math.ceil(target_size / image_size)
 
     # make test data, all with same image path, avoid having to commit 400MB of data to repo
     image_col_name = 'image'
     extra_col_name = 'extra' # dummy column, ensure we aren't loosing columns
     source_directory = tempfile.mkdtemp()
```

### Comparing `arthurai-3.8.8/tests/test_explanation_packager.py` & `arthurai-3.9.0/tests/test_explanation_packager.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_file_upload.py` & `arthurai-3.9.0/tests/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_inferences.py` & `arthurai-3.9.0/tests/test_inferences.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_model_metrics.py` & `arthurai-3.9.0/tests/test_model_metrics.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_models.py` & `arthurai-3.9.0/tests/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import responses
 
 from arthurai import ArthurAI
 from arthurai.common.constants import ValueType, Stage, InputType, OutputType, ImageResponseType, ImageContentType
 from arthurai.core.attributes import AttributeCategory, AttributeBin, ArthurAttribute
 from arthurai.core.models import ArthurModel
 import arthurai.core.util as core_util
+from arthurai.common.exceptions import UserValueError, MethodNotApplicableError
 from tests.base_test import BaseTest
 from tests.test_request_models.fixtures import model_response_json_strings
 
 
 class TestArthurModel(BaseTest):
     @responses.activate
     def test_send_parquet_file(self):
@@ -276,7 +277,40 @@
         open_mock = mock_open()
         with patch("arthurai.core.models.open", open_mock, create=True):
             resulting_file = model.get_image(image_id, path, type=type)
 
         assert resulting_file == expected_image_file
         open_mock.assert_called_with(expected_image_file, 'wb')
         open_mock.return_value.write.assert_called_once_with(response_content)
+
+
+    def test_add_object_detection_output_attributes(self):
+        model = ArthurModel(
+            partner_model_id="test",
+            client=None,
+            input_type=InputType.Image,
+            output_type=OutputType.Multiclass,
+        )
+
+        # cannot call without proper types
+        with pytest.raises(MethodNotApplicableError):
+            model.add_object_detection_output_attributes('pred', 'gt', ['class_1', 'class_2'])
+        model.input_type = InputType.NLP
+        model.output_type = OutputType.ObjectDetection
+        with pytest.raises(MethodNotApplicableError):
+            model.add_object_detection_output_attributes('pred', 'gt', ['class_1', 'class_2'])
+
+        # cannot call without classes
+        model.output_type = OutputType.ObjectDetection
+        model.input_type = InputType.Image
+        with pytest.raises(UserValueError):
+            model.add_object_detection_output_attributes('pred', 'gt', [])
+        
+        # names cannot match
+        with pytest.raises(UserValueError):
+            model.add_object_detection_output_attributes('pred', 'pred', ['class_1', 'class_2'])
+
+        # happy path
+        model.add_object_detection_output_attributes('pred', 'gt', ['class_1', 'class_2'])
+        assert model.get_attribute('pred').value_type == ValueType.BoundingBox
+        assert model.get_attribute('gt').value_type == ValueType.BoundingBox
+        assert model.image_class_labels == ['class_1', 'class_2']
```

### Comparing `arthurai-3.8.8/tests/test_models_service.py` & `arthurai-3.9.0/tests/test_models_service.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_reference_dataset.py` & `arthurai-3.9.0/tests/test_reference_dataset.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_request_models/fixtures.py` & `arthurai-3.9.0/tests/test_request_models/fixtures.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_request_models/test_alert_rule.py` & `arthurai-3.9.0/tests/test_request_models/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `arthurai-3.8.8/tests/test_request_models/test_model.py` & `arthurai-3.9.0/tests/test_request_models/test_model.py`

 * *Files identical despite different names*

