# Comparing `tmp/johnsnowlabs-4.4.8.tar.gz` & `tmp/johnsnowlabs-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.4.8.tar", last modified: Wed Jun 14 20:49:21 2023, max compression
+gzip compressed data, was "johnsnowlabs-4.4.9.tar", last modified: Tue Jul  4 22:09:42 2023, max compression
```

## Comparing `johnsnowlabs-4.4.8.tar` & `johnsnowlabs-4.4.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.205736 johnsnowlabs-4.4.8/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.8/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-06-14 20:49:21.205736 johnsnowlabs-4.4.8/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.8/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.197735 johnsnowlabs-4.4.8/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.8/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.197735 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-06-13 13:24:37.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs-4.4.8/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4755 2023-06-07 00:53:32.000000 johnsnowlabs-4.4.8/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4703 2023-06-07 00:47:56.000000 johnsnowlabs-4.4.8/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4625 2023-06-07 00:48:11.000000 johnsnowlabs-4.4.8/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.8/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31557 2023-06-13 08:46:00.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs-4.4.8/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2241 2023-06-14 20:19:39.000000 johnsnowlabs-4.4.8/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.201736 johnsnowlabs-4.4.8/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-06-14 20:24:15.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.205736 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.8/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.8/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.8/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-06-14 20:49:21.197735 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-06-14 20:49:21.000000 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-06-14 20:49:21.000000 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-06-14 20:49:21.000000 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-06-14 20:49:21.000000 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-06-14 20:49:21.000000 johnsnowlabs-4.4.8/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-06-14 20:49:21.205736 johnsnowlabs-4.4.8/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1900 2023-06-14 20:49:17.000000 johnsnowlabs-4.4.8/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.716014 johnsnowlabs-4.4.9/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.9/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-07-04 22:09:42.716014 johnsnowlabs-4.4.9/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.9/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs-4.4.9/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9794 2023-05-28 18:29:17.000000 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-07-04 19:15:47.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-06-19 13:38:29.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12178 2023-05-26 21:55:38.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-06-06 22:37:19.000000 johnsnowlabs-4.4.9/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4817 2023-07-04 22:05:29.000000 johnsnowlabs-4.4.9/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4765 2023-07-04 22:05:29.000000 johnsnowlabs-4.4.9/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4687 2023-07-04 22:05:29.000000 johnsnowlabs-4.4.9/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs-4.4.9/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4925 2023-05-26 21:57:49.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    33315 2023-07-04 22:09:34.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs-4.4.9/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2202 2023-07-04 22:05:29.000000 johnsnowlabs-4.4.9/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4409 2023-05-26 12:08:46.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10596 2023-07-04 22:00:25.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-06-14 20:24:15.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.716014 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs-4.4.9/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-07-04 21:29:57.000000 johnsnowlabs-4.4.9/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.9/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-07-04 22:09:42.712013 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-07-04 22:09:42.000000 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-07-04 22:09:42.000000 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-07-04 22:09:42.000000 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-07-04 22:09:42.000000 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-07-04 22:09:42.000000 johnsnowlabs-4.4.9/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-07-04 22:09:42.716014 johnsnowlabs-4.4.9/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2054 2023-07-04 19:16:23.000000 johnsnowlabs-4.4.9/setup.py
```

### Comparing `johnsnowlabs-4.4.8/LICENSE` & `johnsnowlabs-4.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/PKG-INFO` & `johnsnowlabs-4.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.8
+Version: 4.4.9
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.8/README.md` & `johnsnowlabs-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/__init__.py` & `johnsnowlabs-4.4.9/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-4.4.9/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-4.4.9/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/finance.py` & `johnsnowlabs-4.4.9/johnsnowlabs/finance.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             Resolution2Chunk,
             ResolverMerger,
             NerTemplateRenderModel,
             AverageEmbeddings,
             Doc2ChunkInternal,
+            Chunk2Token,
+            ExtractiveSummarization,
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/legal.py` & `johnsnowlabs-4.4.9/johnsnowlabs/legal.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,16 @@
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             # Resolution2Chunk,
             ResolverMerger,
             NerTemplateRenderModel,
             AverageEmbeddings,
             Doc2ChunkInternal,
+            Chunk2Token,
+            ExtractiveSummarization,
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
         from sparknlp_jsl import training_log_parser, Deid
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/medical.py` & `johnsnowlabs-4.4.9/johnsnowlabs/medical.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             DocumentMLClassifierApproach,
             DocumentMLClassifierModel,
             Resolution2Chunk,
             MedicalQuestionAnswering,
             NerTemplateRenderModel,
             AverageEmbeddings,
             Doc2ChunkInternal,
+            Chunk2Token,
+            ExtractiveSummarization,
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/nlp.py` & `johnsnowlabs-4.4.9/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-4.4.9/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-4.4.9/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import glob
 import json
 import os
 from pathlib import Path
-from typing import Optional, Union, Dict, List
+from typing import Dict, List, Optional, Union
 
 from pydantic import validator
 
 from johnsnowlabs import settings
 from johnsnowlabs.abstract_base.pydantic_model import WritableBaseModel
 from johnsnowlabs.py_models.lib_version import LibVersion
 from johnsnowlabs.py_models.primitive import LibVersionIdentifier, Secret
 from johnsnowlabs.utils.enums import ProductName
 from johnsnowlabs.utils.file_utils import json_path_as_dict
-from johnsnowlabs.utils.my_jsl_api import (
-    get_user_licenses,
-    download_license,
-    get_access_token,
-    get_access_key_from_browser,
-    get_user_lib_secrets,
-)
+from johnsnowlabs.utils.my_jsl_api import (download_license,
+                                           get_access_key_from_browser,
+                                           get_access_token, get_secrets,
+                                           get_user_lib_secrets,
+                                           get_user_licenses)
 
 secret_json_keys = [
     "JSL_SECRET",
     "SECRET",
     "SPARK_NLP_LICENSE",
     "JSL_LICENSE",
     "JSL_VERSION",
@@ -87,15 +85,15 @@
         try:
             if (
                 not JslSecrets.is_hc_secret_correct_version(HC_SECRET)
                 and not hc_validation_logged
             ):
                 hc_validation_logged = True
                 print(
-                    f"🚨 Outdated Medical Secrets in license file. Version={HC_SECRET.split('-')[0]} but should be Version={settings.raw_version_medical}"
+                    f"🚨 Outdated Medical Secrets in license file. Version={(HC_SECRET.split('-')[0] if HC_SECRET else None)} but should be Version={settings.raw_version_medical}"
                 )
                 if settings.enforce_secret_on_version:
                     raise ValueError("Invalid HC Secret")
                 else:
                     return HC_SECRET
 
             else:
@@ -119,15 +117,15 @@
         try:
             if (
                 not JslSecrets.is_ocr_secret_correct_version(OCR_SECRET)
                 and not ocr_validation_logged
             ):
                 ocr_validation_logged = True
                 print(
-                    f"🚨 Outdated OCR Secrets in license file. Version={OCR_SECRET.split('-')[0]} but should be Version={settings.raw_version_ocr}"
+                    f"🚨 Outdated OCR Secrets in license file. Version={(OCR_SECRET.split('-')[0] if OCR_SECRET else None)} but should be Version={settings.raw_version_ocr}"
                 )
                 if settings.enforce_secret_on_version:
                     raise ValueError("Invalid OCR Secret")
                 else:
                     return OCR_SECRET
             else:
                 return OCR_SECRET
@@ -262,14 +260,20 @@
                 # Try auto Resolve credentials if none are supplied
                 secrets = JslSecrets.search_default_locations(
                     license_number=local_license_number
                 )
             if not secrets and not force_browser:
                 # Search Env Vars
                 secrets = JslSecrets.search_env_vars()
+            
+            if secrets and settings.enforce_versions and not JslSecrets.is_hc_secret_correct_version(secrets.HC_SECRET) and not JslSecrets.is_ocr_secret_correct_version(secrets.OCR_SECRET):
+                # Make sure secrets and versions re enforced
+                print("👷 Trying to install compatible secrets. Use nlp.settings.enforce_versions=False if you want to install outdated secrets.")
+                secrets = JslSecrets.enforce_versions(secrets)
+
         except Exception as err:
             print(
                 f"🚨 Failure Trying to read license {err}\n",
                 f"Trying to use license from John Snow Labs home folder if it exists",
             )
 
         if not secrets and not force_browser:
@@ -467,14 +471,42 @@
             raise FileNotFoundError(f"No file found for secrets_path={secrets_path}")
         f = open(secrets_path, encoding="utf8")
         creds = JslSecrets.from_json_dict(json.load(f))
         f.close()
         return creds
 
     @staticmethod
+    def enforce_versions(data: "JslSecrets") -> "JslSecrets":
+        secrets  = get_secrets(data.HC_LICENSE or data.OCR_LICENSE or data.JSL_FINANCE_LICENSE or data.JSL_LEGAL_LICENSE)
+        # Fix lib secrets in license data to correct version
+        ocr_candidates = list(
+            filter(
+                lambda x: x.version_secret == settings.raw_version_secret_ocr
+                and x.product == ProductName.ocr,
+                secrets,
+            )
+        )
+        hc_handidates = list(
+            filter(
+                lambda x: x.version_secret == settings.raw_version_secret_medical
+                and x.product == ProductName.hc,
+                secrets,
+            )
+        )
+        data.NLP_VERSION = settings.raw_version_nlp
+        if hc_handidates:
+            data.HC_SECRET = hc_handidates[0].secret
+            data.HC_VERSION = hc_handidates[0].version
+        if ocr_candidates:
+            data.OCR_SECRET = ocr_candidates[0].secret
+            data.OCR_VERSION = ocr_candidates[0].version
+
+        return data
+
+    @staticmethod
     def from_access_token(access_token, license_number=0):
         licenses = get_user_licenses(access_token)
         secrets = get_user_lib_secrets(access_token)
         # 1. Oct Secret
         if license_number >= len(licenses) or license_number < 0:
             raise ValueError(
                 f"You have {len(licenses)} in total. Input License Number {license_number} is invalid, up to {len(licenses) - 1} accepted."
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-4.4.9/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-4.4.9/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/settings.py` & `johnsnowlabs-4.4.9/johnsnowlabs/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.8"
-raw_version_nlp = "4.4.1"
+
+raw_version_jsl_lib = "4.4.9"
+raw_version_nlp = "4.4.4"
 raw_version_nlu = "4.2.2"
 
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.4.3"
-raw_version_secret_medical = "4.4.3"
+raw_version_medical = "4.4.4"
+raw_version_secret_medical = "4.4.4"
 
-raw_version_secret_ocr = "4.4.2"
-raw_version_ocr = "4.4.2"
+raw_version_secret_ocr = "4.4.3"
+raw_version_ocr = "4.4.3"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
 
 # Environment
@@ -61,16 +62,15 @@
 db_py_jobs_dir = f"{dbfs_home_dir}/py_jobs"
 db_py_notebook_dir = f"{dbfs_home_dir}/py_notebook_jobs"
 db_jar_jobs_dir = f"{dbfs_home_dir}/jar_jobs"
 
 db_cluster_name = "John-Snow-Labs-Databricks-Auto-Cluster🚀"
 db_driver_node_type = "i3.xlarge"
 db_node_type_id = "i3.xlarge"
-# db_spark_version = "10.5.x-scala2.12"
-db_spark_version = "12.2.x-scala2.12"
+db_spark_version = "10.5.x-scala2.12"
 
 db_job_name = "John-Snow-Labs-Job {job} 🚀"
 db_run_name = "John-Snow-Labs-Run 🚀"
 
 # Local Spark mode
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/enums.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/functional.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/my_jsl_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import hashlib
 import json
 import os
 import random
 import string
 import webbrowser
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from typing import List, Dict
-
+from typing import Dict, List
 # imports related to get access token with PKCE Oauth
 from urllib import parse
 from urllib.request import Request, urlopen
 
 from johnsnowlabs.utils.enums import ProductName
 
+LICENSE_SERVER_ORIGIN = os.environ.get("LICENSE_SERVER_ORIGIN", "https://license.johnsnowlabs.com")
+
 MYJSL_ORIGIN = os.environ.get("MYJSL_ORIGIN", "https://my.johnsnowlabs.com")
 
 # save_path that license should be downloaded there
 LICENSE_PATH = "downloaded-license.json"
 
 
 # using urllib to avoid additional package dependencies like requests
@@ -126,14 +127,26 @@
             ]
         )
         print(f"Cannot login. error={errors}")
         exit(1)
     access_token = data["data"]["getAccessToken"]["ok"]["token"]
     return access_token
 
+def get_secrets(license):
+    try:
+        data = http_request(url=f"{LICENSE_SERVER_ORIGIN}/johnsnowlabs/releases/", method="GET", access_token=license)
+        if data:
+            return [LibSecretResponse(
+                isLatest=r.get("is_latest"),
+                product=r.get("product"),
+                secret=r.get("secret"),
+                version=r.get("version"),
+            ) for r in data]
+    except Exception:
+        raise ValueError("Usage of invalid/expired license.")
 
 def get_user_lib_secrets(access_token):
     secrets_query = """query ReleasesQuery {
 	releases {
 		product
 		version
 		secret
@@ -233,15 +246,15 @@
 
     choice = ensure_correct_choice(len(licenses))
     return licenses[choice]
 
 
 def open_authorized_url(url, in_colab=False):
     if in_colab:
-        from IPython.display import display, Javascript
+        from IPython.display import Javascript, display
 
         display(
             Javascript(
                 """
         var a = document.createElement("a");
         a.id="auth-btn"
         a.setAttribute("target", "_blank");
@@ -317,15 +330,15 @@
                     "redirect_uri": redirect_uri,
                 }
             ),
         )
         open_authorized_url(url, in_colab)
         httpd.handle_request()
         if in_colab:
-            from IPython.display import display, Javascript
+            from IPython.display import Javascript, display
 
             display(Javascript("document.body.removeChild(a);"))
 
     if OauthRequestHandler.code:
         data = http_request(
             f"{MYJSL_ORIGIN}/oauth/token/",
             data={
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-4.4.9/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs/visual.py` & `johnsnowlabs-4.4.9/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-4.4.9/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 4.4.8
+Version: 4.4.9
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs-4.4.8/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-4.4.9/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.4.8/setup.py` & `johnsnowlabs-4.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,29 +19,31 @@
     "databricks-api",
     "pydantic",
     "colorama",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
+    # name='johnsnowlabs_for_databricks',
     name="johnsnowlabs",
-    # name="johnsnowlabs_for_databricks",
     description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
     "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
     long_description_content_type="text/markdown",
     url="https://www.johnsnowlabs.com/",
     author="John Snow Labs",
     author_email="christian@johnsnowlabs.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
     ],
     keywords="Spark NLP OCR Finance Legal Medical John Snow Labs  ",
     packages=find_packages(exclude=["test*", "tmp*"]),  # exclude=['test']
```

