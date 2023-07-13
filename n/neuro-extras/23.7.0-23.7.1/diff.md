# Comparing `tmp/neuro-extras-23.7.0.tar.gz` & `tmp/neuro-extras-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-extras-23.7.0.tar", last modified: Thu Jul  6 20:26:38 2023, max compression
+gzip compressed data, was "neuro-extras-23.7.1.tar", last modified: Thu Jul 13 12:27:09 2023, max compression
```

## Comparing `neuro-extras-23.7.0.tar` & `neuro-extras-23.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/assets/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/merge_docker_auths.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/web.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/image_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/seldon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:26:19.000000 neuro-extras-23.7.0/neuro_extras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-06 20:26:38.831864 neuro-extras-23.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/e2e/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/cloud_to_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/cloud_to_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/local_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/local_to_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/platform_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/test_data_cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_init_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_seldon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.140555 neuro-extras-23.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-13 12:27:09.140555 neuro-extras-23.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.132555 neuro-extras-23.7.1/neuro_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.136555 neuro-extras-23.7.1/neuro_extras/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/assets/merge_docker_auths.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.136555 neuro-extras-23.7.1/neuro_extras/assets/seldon.package/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/assets/seldon.package/seldon.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/assets/seldon.package/seldon_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.136555 neuro-extras-23.7.1/neuro_extras/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/data/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/seldon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/neuro_extras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.136555 neuro-extras-23.7.1/neuro_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:26:46.000000 neuro-extras-23.7.1/neuro_extras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 12:27:09.000000 neuro-extras-23.7.1/neuro_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-13 12:27:09.140555 neuro-extras-23.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.136555 neuro-extras-23.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.140555 neuro-extras-23.7.1/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:27:09.140555 neuro-extras-23.7.1/tests/e2e/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/cloud_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/cloud_to_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/local_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/local_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/platform_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/test_data_cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/test_init_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/test_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-13 12:26:33.000000 neuro-extras-23.7.1/tests/e2e/test_seldon.py
```

### Comparing `neuro-extras-23.7.0/LICENSE` & `neuro-extras-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/README.md` & `neuro-extras-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/__init__.py` & `neuro-extras-23.7.1/neuro_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/assets/merge_docker_auths.sh` & `neuro-extras-23.7.1/neuro_extras/assets/merge_docker_auths.sh`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon.Dockerfile` & `neuro-extras-23.7.1/neuro_extras/assets/seldon.package/seldon.Dockerfile`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon_model.py` & `neuro-extras-23.7.1/neuro_extras/assets/seldon.package/seldon_model.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/cli.py` & `neuro-extras-23.7.1/neuro_extras/cli.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/common.py` & `neuro-extras-23.7.1/neuro_extras/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/config.py` & `neuro-extras-23.7.1/neuro_extras/config.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/__init__.py` & `neuro-extras-23.7.1/neuro_extras/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/archive.py` & `neuro-extras-23.7.1/neuro_extras/data/archive.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/azure.py` & `neuro-extras-23.7.1/neuro_extras/data/azure.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/common.py` & `neuro-extras-23.7.1/neuro_extras/data/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/fs.py` & `neuro-extras-23.7.1/neuro_extras/data/fs.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/gcs.py` & `neuro-extras-23.7.1/neuro_extras/data/gcs.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/local.py` & `neuro-extras-23.7.1/neuro_extras/data/local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/operations.py` & `neuro-extras-23.7.1/neuro_extras/data/operations.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/remote.py` & `neuro-extras-23.7.1/neuro_extras/data/remote.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/s3.py` & `neuro-extras-23.7.1/neuro_extras/data/s3.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/data/web.py` & `neuro-extras-23.7.1/neuro_extras/data/web.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/image.py` & `neuro-extras-23.7.1/neuro_extras/image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/image_builder.py` & `neuro-extras-23.7.1/neuro_extras/image_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 KANIKO_IMAGE_REF = "gcr.io/kaniko-project/executor"
 KANIKO_IMAGE_TAG = "v1.3.0-debug"  # since it has busybox, which is needed for auth
 KANIKO_AUTH_PREFIX = "NE_REGISTRY_AUTH"
 KANIKO_DOCKER_CONFIG_PATH = "/kaniko/.docker/config.json"
 KANIKO_AUTH_SCRIPT_PATH = "/kaniko/.docker/merge_docker_auths.sh"
 KANIKO_CONTEXT_PATH = "/kaniko_context"
+KANIKO_EXTRA_ENVS = ("container=docker",)
 BUILDER_JOB_LIFESPAN = "4h"
 BUILDER_JOB_SHEDULE_TIMEOUT = "20m"
 
 MIN_BUILD_PRESET_CPU: float = 2
 MIN_BUILD_PRESET_MEM: int = 4096
 
 logger = logging.getLogger(__name__)
@@ -288,14 +289,25 @@
         ]
         if job_preset:
             build_command.append(f"--preset={job_preset}")
         for volume in volumes:
             build_command.append(f"--volume={volume}")
         for env in envs:
             build_command.append(f"--env={env}")
+        envs_keys = [e.split("=")[0] for e in envs]
+        for extra_env in KANIKO_EXTRA_ENVS:
+            if extra_env.split("=")[0] in envs_keys:
+                logger.warning(
+                    f"Cannot overwite env {extra_env}: already present. "
+                    "Consider removing this environment variable from your config, "
+                    "otherwise, the build might fail."
+                )
+            else:
+                build_command.append(f"--env={extra_env}")
+
         for build_tag in build_tags:
             build_command.append(f"--tag={build_tag}")
         if entrypoint:
             entrypoint.append(" ".join(kaniko_args))
             build_command.append("--entrypoint")
             build_command.append(f"sh -c {shlex.quote(' '.join(entrypoint))}")
             build_command.append(f"{KANIKO_IMAGE_REF}:{KANIKO_IMAGE_TAG}")
```

### Comparing `neuro-extras-23.7.0/neuro_extras/k8s.py` & `neuro-extras-23.7.1/neuro_extras/k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/main.py` & `neuro-extras-23.7.1/neuro_extras/main.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/seldon.py` & `neuro-extras-23.7.1/neuro_extras/seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras/utils.py` & `neuro-extras-23.7.1/neuro_extras/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/neuro_extras.egg-info/SOURCES.txt` & `neuro-extras-23.7.1/neuro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/pyproject.toml` & `neuro-extras-23.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/setup.cfg` & `neuro-extras-23.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/setup.py` & `neuro-extras-23.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/conftest.py` & `neuro-extras-23.7.1/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/cloud_to_local.py` & `neuro-extras-23.7.1/tests/e2e/data/cloud_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/cloud_to_platform.py` & `neuro-extras-23.7.1/tests/e2e/data/cloud_to_platform.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/local_to_cloud.py` & `neuro-extras-23.7.1/tests/e2e/data/local_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/local_to_local.py` & `neuro-extras-23.7.1/tests/e2e/data/local_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/platform_to_cloud.py` & `neuro-extras-23.7.1/tests/e2e/data/platform_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/resources.py` & `neuro-extras-23.7.1/tests/e2e/data/resources.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/test_data_cp.py` & `neuro-extras-23.7.1/tests/e2e/data/test_data_cp.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/data/test_data_transfer.py` & `neuro-extras-23.7.1/tests/e2e/data/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/test_image.py` & `neuro-extras-23.7.1/tests/e2e/test_image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/test_k8s.py` & `neuro-extras-23.7.1/tests/e2e/test_k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-23.7.0/tests/e2e/test_seldon.py` & `neuro-extras-23.7.1/tests/e2e/test_seldon.py`

 * *Files identical despite different names*

