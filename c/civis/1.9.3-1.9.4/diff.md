# Comparing `tmp/civis-1.9.3.tar.gz` & `tmp/civis-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/civis-1.9.3.tar", last modified: Tue Feb  5 21:48:37 2019, max compression
+gzip compressed data, was "dist/civis-1.9.4.tar", last modified: Thu Feb 28 22:08:31 2019, max compression
```

## Comparing `civis-1.9.3.tar` & `civis-1.9.4.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/
--rw-r--r--   0 lsander    (501) staff       (20)     9097 2019-02-05 21:48:37.000000 civis-1.9.3/PKG-INFO
--rw-r--r--   0 lsander    (501) staff       (20)     1501 2017-08-10 18:36:45.000000 civis-1.9.3/LICENSE.md
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis.egg-info/
--rw-r--r--   0 lsander    (501) staff       (20)     9097 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/PKG-INFO
--rw-r--r--   0 lsander    (501) staff       (20)     1348 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/SOURCES.txt
--rw-r--r--   0 lsander    (501) staff       (20)      100 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/entry_points.txt
--rw-r--r--   0 lsander    (501) staff       (20)      297 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/requires.txt
--rw-r--r--   0 lsander    (501) staff       (20)        6 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/top_level.txt
--rw-r--r--   0 lsander    (501) staff       (20)        1 2019-02-05 21:48:36.000000 civis-1.9.3/civis.egg-info/dependency_links.txt
--rw-r--r--   0 lsander    (501) staff       (20)      344 2019-02-04 19:22:57.000000 civis-1.9.3/requirements.txt
--rw-r--r--   0 lsander    (501) staff       (20)      178 2017-10-03 18:58:16.000000 civis-1.9.3/MANIFEST.in
--rw-r--r--   0 lsander    (501) staff       (20)     2517 2019-02-04 17:56:42.000000 civis-1.9.3/setup.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/
--rw-r--r--   0 lsander    (501) staff       (20)     2754 2017-11-20 22:22:50.000000 civis-1.9.3/civis/compat.py
--rw-r--r--   0 lsander    (501) staff       (20)      413 2017-08-10 18:36:45.000000 civis-1.9.3/civis/pubnub.py
--rw-r--r--   0 lsander    (501) staff       (20)       22 2019-02-05 21:46:11.000000 civis-1.9.3/civis/_version.py
--rw-r--r--   0 lsander    (501) staff       (20)     2660 2018-05-17 17:46:16.000000 civis-1.9.3/civis/_deprecation.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/resources/
--rw-r--r--   0 lsander    (501) staff       (20)      425 2017-10-03 18:58:16.000000 civis-1.9.3/civis/resources/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)    21655 2018-05-17 17:46:16.000000 civis-1.9.3/civis/resources/_resources.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/io/
--rw-r--r--   0 lsander    (501) staff       (20)     5716 2018-05-17 17:46:16.000000 civis-1.9.3/civis/io/_databases.py
--rw-r--r--   0 lsander    (501) staff       (20)    42712 2019-01-10 18:48:59.000000 civis-1.9.3/civis/io/_tables.py
--rw-r--r--   0 lsander    (501) staff       (20)      185 2017-08-10 18:36:45.000000 civis-1.9.3/civis/io/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)    16709 2019-01-10 18:48:59.000000 civis-1.9.3/civis/io/_files.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/tests/
--rw-r--r--   0 lsander    (501) staff       (20)    14921 2017-11-20 22:22:51.000000 civis-1.9.3/civis/tests/test_resources.py
--rw-r--r--   0 lsander    (501) staff       (20)     2733 2017-11-20 22:22:51.000000 civis-1.9.3/civis/tests/test_utils.py
--rw-r--r--   0 lsander    (501) staff       (20)     5442 2017-09-19 21:01:12.000000 civis-1.9.3/civis/tests/test_response.py
--rw-r--r--   0 lsander    (501) staff       (20)     1465 2017-08-10 18:36:45.000000 civis-1.9.3/civis/tests/testcase.py
--rw-r--r--   0 lsander    (501) staff       (20)    18162 2018-03-05 16:04:19.000000 civis-1.9.3/civis/tests/test_futures.py
--rw-r--r--   0 lsander    (501) staff       (20)       68 2017-10-03 18:58:16.000000 civis-1.9.3/civis/tests/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)      487 2017-10-03 18:58:16.000000 civis-1.9.3/civis/tests/test_mocks.py
--rw-r--r--   0 lsander    (501) staff       (20)    23475 2019-01-10 18:48:59.000000 civis-1.9.3/civis/tests/test_io.py
--rw-r--r--   0 lsander    (501) staff       (20)     3221 2017-08-10 18:36:45.000000 civis-1.9.3/civis/tests/petstore.json
--rw-r--r--   0 lsander    (501) staff       (20)    19629 2018-01-18 17:06:29.000000 civis-1.9.3/civis/tests/test_parallel.py
--rw-r--r--   0 lsander    (501) staff       (20)      537 2017-11-20 22:22:51.000000 civis-1.9.3/civis/tests/test_compat.py
--rw-r--r--   0 lsander    (501) staff       (20)  2070045 2019-02-05 21:46:11.000000 civis-1.9.3/civis/tests/civis_api_spec_channels.json
--rw-r--r--   0 lsander    (501) staff       (20)     2140 2018-05-17 17:46:16.000000 civis-1.9.3/civis/tests/test_deprecate.py
--rw-r--r--   0 lsander    (501) staff       (20)  2068020 2019-02-05 21:46:11.000000 civis-1.9.3/civis/tests/civis_api_spec.json
--rw-r--r--   0 lsander    (501) staff       (20)     1398 2017-10-03 18:58:16.000000 civis-1.9.3/civis/tests/test_client.py
--rw-r--r--   0 lsander    (501) staff       (20)     4224 2019-02-05 21:46:11.000000 civis-1.9.3/civis/tests/test_cli.py
--rw-r--r--   0 lsander    (501) staff       (20)      665 2017-08-10 18:36:45.000000 civis-1.9.3/civis/tests/test_base.py
--rw-r--r--   0 lsander    (501) staff       (20)     3573 2018-07-30 17:36:50.000000 civis-1.9.3/civis/tests/test_polling.py
--rw-r--r--   0 lsander    (501) staff       (20)     1415 2018-05-17 17:46:16.000000 civis-1.9.3/civis/tests/mocks.py
--rw-r--r--   0 lsander    (501) staff       (20)      259 2017-08-29 21:54:17.000000 civis-1.9.3/civis/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)     6363 2017-09-19 21:01:12.000000 civis-1.9.3/civis/response.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/utils/
--rw-r--r--   0 lsander    (501) staff       (20)       50 2017-08-10 18:36:45.000000 civis-1.9.3/civis/utils/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)     1015 2018-05-17 17:46:16.000000 civis-1.9.3/civis/utils/_jobs.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/cli/
--rw-r--r--   0 lsander    (501) staff       (20)       73 2017-08-10 18:36:45.000000 civis-1.9.3/civis/cli/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)     5526 2018-01-24 19:42:57.000000 civis-1.9.3/civis/cli/_cli_commands.py
--rwxr-xr-x   0 lsander    (501) staff       (20)    11341 2018-01-03 21:35:42.000000 civis-1.9.3/civis/cli/__main__.py
--rw-r--r--   0 lsander    (501) staff       (20)    28092 2018-05-17 17:46:16.000000 civis-1.9.3/civis/futures.py
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/ml/
-drwxr-xr-x   0 lsander    (501) staff       (20)        0 2019-02-05 21:48:37.000000 civis-1.9.3/civis/ml/tests/
--rw-r--r--   0 lsander    (501) staff       (20)    39390 2019-02-05 21:46:11.000000 civis-1.9.3/civis/ml/tests/test_model.py
--rw-r--r--   0 lsander    (501) staff       (20)        0 2017-11-20 22:22:50.000000 civis-1.9.3/civis/ml/tests/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)       71 2017-08-10 18:36:45.000000 civis-1.9.3/civis/ml/__init__.py
--rw-r--r--   0 lsander    (501) staff       (20)    62356 2019-02-05 21:46:11.000000 civis-1.9.3/civis/ml/_model.py
--rwxr-xr-x   0 lsander    (501) staff       (20)     4292 2017-11-01 15:28:54.000000 civis-1.9.3/civis/run_joblib_func.py
--rw-r--r--   0 lsander    (501) staff       (20)     8484 2017-11-20 22:22:50.000000 civis-1.9.3/civis/polling.py
--rw-r--r--   0 lsander    (501) staff       (20)    40356 2018-05-17 17:46:16.000000 civis-1.9.3/civis/parallel.py
--rw-r--r--   0 lsander    (501) staff       (20)     7709 2017-11-20 22:22:50.000000 civis-1.9.3/civis/base.py
--rw-r--r--   0 lsander    (501) staff       (20)     4673 2018-01-03 21:35:42.000000 civis-1.9.3/civis/_utils.py
--rw-r--r--   0 lsander    (501) staff       (20)    13532 2018-05-17 17:46:16.000000 civis-1.9.3/civis/civis.py
--rw-r--r--   0 lsander    (501) staff       (20)       99 2019-02-05 21:48:37.000000 civis-1.9.3/setup.cfg
--rw-r--r--   0 lsander    (501) staff       (20)     6657 2019-02-04 17:56:42.000000 civis-1.9.3/README.rst
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/
+-rw-r--r--   0 mheilman   (502) staff       (20)     9097 2019-02-28 22:08:31.000000 civis-1.9.4/PKG-INFO
+-rw-r--r--   0 mheilman   (502) staff       (20)     1501 2017-04-05 14:45:03.000000 civis-1.9.4/LICENSE.md
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/
+-rw-r--r--   0 mheilman   (502) staff       (20)     9097 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/PKG-INFO
+-rw-r--r--   0 mheilman   (502) staff       (20)     1374 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/SOURCES.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)      100 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/entry_points.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)      297 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/requires.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)        6 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/top_level.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)        1 2019-02-28 22:08:31.000000 civis-1.9.4/civis.egg-info/dependency_links.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)      344 2017-10-13 15:03:53.000000 civis-1.9.4/requirements.txt
+-rw-r--r--   0 mheilman   (502) staff       (20)      178 2017-10-13 15:03:53.000000 civis-1.9.4/MANIFEST.in
+-rw-r--r--   0 mheilman   (502) staff       (20)     2517 2019-02-07 15:06:59.000000 civis-1.9.4/setup.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/
+-rw-r--r--   0 mheilman   (502) staff       (20)     2754 2018-03-13 15:42:03.000000 civis-1.9.4/civis/compat.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      413 2017-04-05 14:45:03.000000 civis-1.9.4/civis/pubnub.py
+-rw-r--r--   0 mheilman   (502) staff       (20)       22 2019-02-28 22:06:09.000000 civis-1.9.4/civis/_version.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     2660 2018-04-12 19:51:26.000000 civis-1.9.4/civis/_deprecation.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/resources/
+-rw-r--r--   0 mheilman   (502) staff       (20)      425 2017-10-13 15:03:53.000000 civis-1.9.4/civis/resources/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    21655 2018-04-18 16:25:07.000000 civis-1.9.4/civis/resources/_resources.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/io/
+-rw-r--r--   0 mheilman   (502) staff       (20)     5716 2018-04-12 19:51:26.000000 civis-1.9.4/civis/io/_databases.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    42712 2018-11-30 18:10:19.000000 civis-1.9.4/civis/io/_tables.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      185 2017-06-29 13:59:33.000000 civis-1.9.4/civis/io/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    16709 2018-12-03 17:53:14.000000 civis-1.9.4/civis/io/_files.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/tests/
+-rw-r--r--   0 mheilman   (502) staff       (20)    14921 2017-11-14 23:00:55.000000 civis-1.9.4/civis/tests/test_resources.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     2733 2017-11-14 22:41:19.000000 civis-1.9.4/civis/tests/test_utils.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     5556 2019-02-28 19:44:50.000000 civis-1.9.4/civis/tests/test_response.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     1465 2017-04-05 14:45:03.000000 civis-1.9.4/civis/tests/testcase.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    18162 2018-03-13 14:47:28.000000 civis-1.9.4/civis/tests/test_futures.py
+-rw-r--r--   0 mheilman   (502) staff       (20)       68 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      804 2019-02-28 15:46:05.000000 civis-1.9.4/civis/tests/test_civis.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      487 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/test_mocks.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    23475 2018-12-03 17:53:14.000000 civis-1.9.4/civis/tests/test_io.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     3221 2017-04-05 14:45:03.000000 civis-1.9.4/civis/tests/petstore.json
+-rw-r--r--   0 mheilman   (502) staff       (20)    19629 2018-01-24 15:33:19.000000 civis-1.9.4/civis/tests/test_parallel.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      537 2017-11-14 23:00:55.000000 civis-1.9.4/civis/tests/test_compat.py
+-rw-r--r--   0 mheilman   (502) staff       (20)  2070045 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/civis_api_spec_channels.json
+-rw-r--r--   0 mheilman   (502) staff       (20)     2140 2018-04-12 19:51:26.000000 civis-1.9.4/civis/tests/test_deprecate.py
+-rw-r--r--   0 mheilman   (502) staff       (20)  2068020 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/civis_api_spec.json
+-rw-r--r--   0 mheilman   (502) staff       (20)     1398 2017-10-13 15:03:53.000000 civis-1.9.4/civis/tests/test_client.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     4224 2019-02-07 15:06:59.000000 civis-1.9.4/civis/tests/test_cli.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      665 2017-06-29 13:59:33.000000 civis-1.9.4/civis/tests/test_base.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     3573 2018-09-24 13:52:12.000000 civis-1.9.4/civis/tests/test_polling.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     1415 2018-04-12 19:51:26.000000 civis-1.9.4/civis/tests/mocks.py
+-rw-r--r--   0 mheilman   (502) staff       (20)      259 2017-10-13 15:03:53.000000 civis-1.9.4/civis/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     6352 2019-02-28 19:44:50.000000 civis-1.9.4/civis/response.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/utils/
+-rw-r--r--   0 mheilman   (502) staff       (20)       50 2017-04-05 14:45:03.000000 civis-1.9.4/civis/utils/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     1015 2018-04-12 19:51:26.000000 civis-1.9.4/civis/utils/_jobs.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/cli/
+-rw-r--r--   0 mheilman   (502) staff       (20)       73 2017-04-05 14:45:03.000000 civis-1.9.4/civis/cli/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     5526 2018-02-01 14:15:15.000000 civis-1.9.4/civis/cli/_cli_commands.py
+-rwxr-xr-x   0 mheilman   (502) staff       (20)    11341 2018-04-18 16:25:23.000000 civis-1.9.4/civis/cli/__main__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    28092 2018-04-12 19:51:26.000000 civis-1.9.4/civis/futures.py
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/ml/
+drwxr-xr-x   0 mheilman   (502) staff       (20)        0 2019-02-28 22:08:31.000000 civis-1.9.4/civis/ml/tests/
+-rw-r--r--   0 mheilman   (502) staff       (20)    39390 2019-02-07 15:06:59.000000 civis-1.9.4/civis/ml/tests/test_model.py
+-rw-r--r--   0 mheilman   (502) staff       (20)        0 2017-11-14 23:00:55.000000 civis-1.9.4/civis/ml/tests/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)       71 2017-06-29 13:59:33.000000 civis-1.9.4/civis/ml/__init__.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    62356 2019-02-07 15:06:59.000000 civis-1.9.4/civis/ml/_model.py
+-rwxr-xr-x   0 mheilman   (502) staff       (20)     4292 2017-10-13 15:03:53.000000 civis-1.9.4/civis/run_joblib_func.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     8484 2017-11-14 23:00:55.000000 civis-1.9.4/civis/polling.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    40356 2018-04-12 19:51:26.000000 civis-1.9.4/civis/parallel.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     7709 2017-11-15 16:50:42.000000 civis-1.9.4/civis/base.py
+-rw-r--r--   0 mheilman   (502) staff       (20)     4673 2018-01-24 15:33:19.000000 civis-1.9.4/civis/_utils.py
+-rw-r--r--   0 mheilman   (502) staff       (20)    13632 2019-02-28 15:46:05.000000 civis-1.9.4/civis/civis.py
+-rw-r--r--   0 mheilman   (502) staff       (20)       99 2019-02-28 22:08:31.000000 civis-1.9.4/setup.cfg
+-rw-r--r--   0 mheilman   (502) staff       (20)     6657 2019-02-07 15:06:59.000000 civis-1.9.4/README.rst
```

### Comparing `civis-1.9.3/PKG-INFO` & `civis-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: civis
-Version: 1.9.3
+Version: 1.9.4
 Summary: Access the Civis Platform API
 Home-page: https://www.civisanalytics.com
 Author: Civis Analytics Inc
 Author-email: opensource@civisanalytics.com
 License: UNKNOWN
 Description: Civis API Python Client
         =======================
```

### Comparing `civis-1.9.3/LICENSE.md` & `civis-1.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis.egg-info/PKG-INFO` & `civis-1.9.4/civis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: civis
-Version: 1.9.3
+Version: 1.9.4
 Summary: Access the Civis Platform API
 Home-page: https://www.civisanalytics.com
 Author: Civis Analytics Inc
 Author-email: opensource@civisanalytics.com
 License: UNKNOWN
 Description: Civis API Python Client
         =======================
```

### Comparing `civis-1.9.3/civis.egg-info/SOURCES.txt` & `civis-1.9.4/civis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 civis/resources/_resources.py
 civis/tests/__init__.py
 civis/tests/civis_api_spec.json
 civis/tests/civis_api_spec_channels.json
 civis/tests/mocks.py
 civis/tests/petstore.json
 civis/tests/test_base.py
+civis/tests/test_civis.py
 civis/tests/test_cli.py
 civis/tests/test_client.py
 civis/tests/test_compat.py
 civis/tests/test_deprecate.py
 civis/tests/test_futures.py
 civis/tests/test_io.py
 civis/tests/test_mocks.py
```

### Comparing `civis-1.9.3/setup.py` & `civis-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/compat.py` & `civis-1.9.4/civis/compat.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/_deprecation.py` & `civis-1.9.4/civis/_deprecation.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/resources/_resources.py` & `civis-1.9.4/civis/resources/_resources.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/io/_databases.py` & `civis-1.9.4/civis/io/_databases.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/io/_tables.py` & `civis-1.9.4/civis/io/_tables.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/io/_files.py` & `civis-1.9.4/civis/io/_files.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_resources.py` & `civis-1.9.4/civis/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_utils.py` & `civis-1.9.4/civis/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_response.py` & `civis-1.9.4/civis/tests/test_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     mock_response.status_code = 200
     return mock_response
 
 
 def _create_empty_response(code, headers):
     mock_response = mock.MagicMock(spec=requests.Response)
     mock_response.status_code = code
+    mock_response.content = b''
     mock_response.headers = headers
     return mock_response
 
 
 def _make_paginated_response(path, params):
     results = [
         [
@@ -97,15 +98,16 @@
 
 def test_response_to_json_no_error():
     raw_response = _create_mock_response({'key': 'value'}, None)
     assert _response_to_json(raw_response) == {'key': 'value'}
 
 
 def test_response_to_no_content_snake():
-    for code in [204, 205]:
+    # Test empty response handling for codes where we're likely to see them.
+    for code in [202, 204, 205]:
         raw_response = _create_empty_response(code, {'header1': 'val1'})
         data = convert_response_data_type(raw_response, return_type='snake')
 
         assert isinstance(data, Response)
         assert data.json_data is None
         assert data.headers == {'header1': 'val1'}
```

### Comparing `civis-1.9.3/civis/tests/testcase.py` & `civis-1.9.4/civis/tests/testcase.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_futures.py` & `civis-1.9.4/civis/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_io.py` & `civis-1.9.4/civis/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/petstore.json` & `civis-1.9.4/civis/tests/petstore.json`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_parallel.py` & `civis-1.9.4/civis/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_compat.py` & `civis-1.9.4/civis/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/civis_api_spec_channels.json` & `civis-1.9.4/civis/tests/civis_api_spec_channels.json`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_deprecate.py` & `civis-1.9.4/civis/tests/test_deprecate.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/civis_api_spec.json` & `civis-1.9.4/civis/tests/civis_api_spec.json`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_client.py` & `civis-1.9.4/civis/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_cli.py` & `civis-1.9.4/civis/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_base.py` & `civis-1.9.4/civis/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/test_polling.py` & `civis-1.9.4/civis/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/tests/mocks.py` & `civis-1.9.4/civis/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/response.py` & `civis-1.9.4/civis/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         content.
 
     Raises
     ------
     CivisClientError
         If the data in the raw response cannot be parsed.
     """
-    if response.status_code in [204, 205]:
+    if response.content == b'':
         return None
     else:
         try:
             return response.json()
         except ValueError:
             raise CivisClientError("Unable to parse JSON from response",
                                    response)
```

### Comparing `civis-1.9.3/civis/utils/_jobs.py` & `civis-1.9.4/civis/utils/_jobs.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/cli/_cli_commands.py` & `civis-1.9.4/civis/cli/_cli_commands.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/cli/__main__.py` & `civis-1.9.4/civis/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/futures.py` & `civis-1.9.4/civis/futures.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/ml/tests/test_model.py` & `civis-1.9.4/civis/ml/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/ml/_model.py` & `civis-1.9.4/civis/ml/_model.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/run_joblib_func.py` & `civis-1.9.4/civis/run_joblib_func.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/polling.py` & `civis-1.9.4/civis/polling.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/parallel.py` & `civis-1.9.4/civis/parallel.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/base.py` & `civis-1.9.4/civis/base.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/_utils.py` & `civis-1.9.4/civis/_utils.py`

 * *Files identical despite different names*

### Comparing `civis-1.9.3/civis/civis.py` & `civis-1.9.4/civis/civis.py`

 * *Files 6% similar despite different names*

```diff
@@ -248,40 +248,46 @@
     @lru_cache(maxsize=128)
     def get_table_id(self, table, database):
         """Return the table ID for a given database and table name.
 
         Parameters
         ----------
         table : str
-            The name of the table in format schema.table.
+            The name of the table in format schema.tablename.
+            Either schema or tablename, or both, can be double-quoted to
+            correctly parse special characters (such as '.').
         database : str or int
             The name or ID of the database.
 
         Returns
         -------
         table_id : int
-            The ID of the table. Only returns exact match to specified
-            table.
+            The ID of the table.
 
         Raises
         ------
         ValueError
-            If an exact table match can't be found.
+            If a table match can't be found.
+
+        Examples
+        --------
+        >>> import civis
+        >>> client = civis.APIClient()
+        >>> client.get_table_id('foo.bar', 'redshift-general')
+        123
+        >>> client.get_table_id('"schema.has.periods".bar', 'redshift-general')
+        456
         """
         database_id = self.get_database_id(database)
         schema, name = civis.io.split_schema_tablename(table)
         tables = self.tables.list(database_id=database_id, schema=schema,
                                   name=name)
         if not tables:
             msg = "No tables found for {} in database {}"
             raise ValueError(msg.format(table, database))
-        found_table = ".".join((tables[0].schema, tables[0].name))
-        if table != found_table:
-            msg = "Given table {} is not an exact match for returned table {}."
-            raise ValueError(msg.format(table, found_table))
 
         return tables[0].id
 
     @property
     @lru_cache(maxsize=128)
     def default_credential(self):
         """The current user's default credential."""
```

### Comparing `civis-1.9.3/README.rst` & `civis-1.9.4/README.rst`

 * *Files identical despite different names*

