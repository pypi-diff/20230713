# Comparing `tmp/edc-rx-0.1.6.tar.gz` & `tmp/edc-rx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-rx-0.1.6.tar", last modified: Wed May 24 15:54:51 2023, max compression
+gzip compressed data, was "edc-rx-0.1.7.tar", last modified: Wed Jul 12 23:51:00 2023, max compression
```

## Comparing `edc-rx-0.1.6.tar` & `edc-rx-0.1.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.878319 edc-rx-0.1.6/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.870007 edc-rx-0.1.6/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.873159 edc-rx-0.1.6/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.6/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.6/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.6/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.6/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-05-24 15:54:51.878397 edc-rx-0.1.6/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.6/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.874005 edc-rx-0.1.6/edc_rx/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.875227 edc-rx-0.1.6/edc_rx/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.6/edc_rx/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.875883 edc-rx-0.1.6/edc_rx/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1698 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/model_mixins/drug_refill_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/model_mixins/drug_supply_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/model_mixins/treatment_pay_methods.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876366 edc-rx-0.1.6/edc_rx/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:41:25.000000 edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876637 edc-rx-0.1.6/edc_rx/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.876866 edc-rx-0.1.6/edc_rx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.6/edc_rx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.877915 edc-rx-0.1.6/edc_rx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.878136 edc-rx-0.1.6/edc_rx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.6/edc_rx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4232 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/tests/tests/test_utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.6/edc_rx/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      799 2023-04-25 02:49:23.000000 edc-rx-0.1.6/edc_rx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 15:54:51.874858 edc-rx-0.1.6/edc_rx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.6/edc_rx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-05-24 15:54:51.000000 edc-rx-0.1.6/edc_rx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.6/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.6/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-05-24 15:54:51.878695 edc-rx-0.1.6/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970413 edc-rx-0.1.7/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.961844 edc-rx-0.1.7/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.965728 edc-rx-0.1.7/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 15:54:44.000000 edc-rx-0.1.7/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-24 15:54:44.000000 edc-rx-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-29 04:55:26.000000 edc-rx-0.1.7/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-29 03:26:32.000000 edc-rx-0.1.7/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-29 04:55:26.000000 edc-rx-0.1.7/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-07-12 23:51:00.970514 edc-rx-0.1.7/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      613 2022-11-29 04:55:26.000000 edc-rx-0.1.7/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.966646 edc-rx-0.1.7/edc_rx/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.967700 edc-rx-0.1.7/edc_rx/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5179 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-29 06:36:26.000000 edc-rx-0.1.7/edc_rx/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968276 edc-rx-0.1.7/edc_rx/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      181 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1612 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/model_mixins/drug_refill_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/model_mixins/drug_supply_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2023-04-18 01:41:25.000000 edc-rx-0.1.7/edc_rx/model_mixins/treatment_pay_methods.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968661 edc-rx-0.1.7/edc_rx/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1237 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.968908 edc-rx-0.1.7/edc_rx/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2047 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.969011 edc-rx-0.1.7/edc_rx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.7/edc_rx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970077 edc-rx-0.1.7/edc_rx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.970300 edc-rx-0.1.7/edc_rx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-03-31 01:06:02.000000 edc-rx-0.1.7/edc_rx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4204 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/tests/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-11-29 04:55:26.000000 edc-rx-0.1.7/edc_rx/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      757 2023-07-12 23:50:53.000000 edc-rx-0.1.7/edc_rx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:51:00.967329 edc-rx-0.1.7/edc_rx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1487 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1335 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-29 04:55:34.000000 edc-rx-0.1.7/edc_rx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-07-12 23:51:00.000000 edc-rx-0.1.7/edc_rx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 15:54:44.000000 edc-rx-0.1.7/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1106 2023-03-31 01:08:39.000000 edc-rx-0.1.7/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-07-12 23:51:00.970837 edc-rx-0.1.7/setup.cfg
```

### Comparing `edc-rx-0.1.6/.github/workflows/build.yml` & `edc-rx-0.1.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/.gitignore` & `edc-rx-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/.pre-commit-config.yaml` & `edc-rx-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/LICENSE` & `edc-rx-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/PKG-INFO` & `edc-rx-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.6/README.rst` & `edc-rx-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/migrations/0001_initial.py` & `edc-rx-0.1.7/edc_rx/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/model_mixins/drug_refill_model_mixin.py` & `edc-rx-0.1.7/edc_rx/model_mixins/drug_refill_model_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,14 @@
     modifications_reason_other = models.CharField(
         verbose_name="If other, please specify ...",
         max_length=150,
         null=True,
         blank=True,
     )
 
-    return_in_days = models.IntegerField(
-        verbose_name=(
-            "In how many days has the patient been asked "
-            "to return to clinic for a drug refill?"
-        ),
-        validators=[MinValueValidator(0), MaxValueValidator(180)],
+    rx_days = models.IntegerField(
+        verbose_name=("Number of days of medication prescribed?"),
+        validators=[MinValueValidator(0), MaxValueValidator(186)],
     )
 
     class Meta:
         abstract = True
```

### Comparing `edc-rx-0.1.6/edc_rx/model_mixins/drug_supply_model_mixin.py` & `edc-rx-0.1.7/edc_rx/model_mixins/drug_supply_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/model_mixins/treatment_pay_methods.py` & `edc-rx-0.1.7/edc_rx/model_mixins/treatment_pay_methods.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py` & `edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_refill_admin_mixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from django.utils.html import format_html
 from django_audit_fields.admin import audit_fieldset_tuple
 from edc_crf.admin import crf_status_fieldset_tuple
 
 
 class DrugRefillAdminMixin:
     form = None
+
     inlines = []
 
+    fieldsets_move_to_end = [crf_status_fieldset_tuple[0], audit_fieldset_tuple[0]]
+
     additional_instructions = format_html(
         '<span style="color:orange">Note: Medications CRF must be completed first.</span>'
     )
 
     fieldsets = (
         (None, {"fields": ("subject_visit", "report_datetime")}),
         (
@@ -21,15 +24,15 @@
                     "rx",
                     "rx_other",
                     "rx_modified",
                     "modifications",
                     "modifications_other",
                     "modifications_reason",
                     "modifications_reason_other",
-                    "return_in_days",
+                    "rx_days",
                 )
             },
         ),
         crf_status_fieldset_tuple,
         audit_fieldset_tuple,
     )
     filter_horizontal = ["rx", "modifications", "modifications_reason"]
```

### Comparing `edc-rx-0.1.6/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py` & `edc-rx-0.1.7/edc_rx/modeladmin_mixins/drug_supply_inline_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class DrugSupplyInlineMixin:
     extra = 1
     view_on_site = False
 
     min_num = 1
-    insert_after = "return_in_days"
+    insert_after = "rx_days"
 
     fieldsets = (
         [
             "Drug Supply",
             {
                 "description": (
                     "For each drug, please state for many days supply "
```

### Comparing `edc-rx-0.1.6/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py` & `edc-rx-0.1.7/edc_rx/modelform_mixins/drug_supply_ncd_modelform_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     def clean(self):
         cleaned_data = super().clean()
         data = dict(self.data.lists())
         rx = self.list_model_cls.objects.filter(id__in=data.get("rx") or [])
         rx_names = [obj.display_name for obj in rx]
         inline_drug_names = self.raise_on_duplicates()
 
-        if data.get("return_in_days")[0] is not None and data.get("return_in_days")[0] != "":
+        if data.get("rx_days")[0] is not None and data.get("rx_days")[0] != "":
             try:
-                validate_total_days(self, return_in_days=int(data.get("return_in_days")[0]))
+                validate_total_days(self, rx_days=int(data.get("rx_days")[0]))
             except TotalDaysMismatch as e:
                 raise forms.ValidationError(e)
 
         if (
             self.cleaned_data.get("drug")
             and self.cleaned_data.get("drug").display_name not in rx_names
         ):
```

### Comparing `edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-local-private.pem` & `edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/tests/etc/user-rsa-restricted-private.pem` & `edc-rx-0.1.7/edc_rx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/edc_rx/tests/tests/test_utils.py` & `edc-rx-0.1.7/edc_rx/tests/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             purchased_days = invalid_combo[2]
             with self.subTest(
                 clinic_days=clinic_days,
                 club_days=club_days,
                 purchased_days=purchased_days,
             ):
                 form.cleaned_data = {
-                    "return_in_days": 30,
+                    "rx_days": 30,
                     "clinic_days": clinic_days,
                     "club_days": club_days,
                     "purchased_days": purchased_days,
                 }
                 with self.assertRaises(TotalDaysMismatch):
                     validate_total_days(form=form)
 
@@ -55,15 +55,15 @@
             purchased_days = valid_combo[2]
             with self.subTest(
                 clinic_days=clinic_days,
                 club_days=club_days,
                 purchased_days=purchased_days,
             ):
                 form.cleaned_data = {
-                    "return_in_days": 30,
+                    "rx_days": 30,
                     "clinic_days": clinic_days,
                     "club_days": club_days,
                     "purchased_days": purchased_days,
                 }
                 try:
                     validate_total_days(form=form)
                 except TotalDaysMismatch as e:
@@ -85,15 +85,15 @@
             purchased_days = invalid_combo[2]
             with self.subTest(
                 clinic_days=clinic_days,
                 club_days=club_days,
                 purchased_days=purchased_days,
             ):
                 form.cleaned_data = {
-                    "return_in_days": 0,
+                    "rx_days": 0,
                     "clinic_days": clinic_days,
                     "club_days": club_days,
                     "purchased_days": purchased_days,
                 }
                 with self.assertRaises(TotalDaysMismatch):
                     validate_total_days(form=form)
 
@@ -110,15 +110,15 @@
             purchased_days = valid_combo[2]
             with self.subTest(
                 clinic_days=clinic_days,
                 club_days=club_days,
                 purchased_days=purchased_days,
             ):
                 form.cleaned_data = {
-                    "return_in_days": 0,
+                    "rx_days": 0,
                     "clinic_days": clinic_days,
                     "club_days": club_days,
                     "purchased_days": purchased_days,
                 }
                 try:
                     validate_total_days(form=form)
                 except TotalDaysMismatch as e:
```

### Comparing `edc-rx-0.1.6/edc_rx.egg-info/PKG-INFO` & `edc-rx-0.1.7/edc_rx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-rx
-Version: 0.1.6
+Version: 0.1.7
 Summary: Medications refill and supply model/form mixins for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-rx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc rx-refill,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-rx-0.1.6/edc_rx.egg-info/SOURCES.txt` & `edc-rx-0.1.7/edc_rx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/pyproject.toml` & `edc-rx-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/runtests.py` & `edc-rx-0.1.7/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-rx-0.1.6/setup.cfg` & `edc-rx-0.1.7/setup.cfg`

 * *Files identical despite different names*

