# Comparing `tmp/cloudfoundry-client-1.8.0.tar.gz` & `tmp/cloudfoundry-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudfoundry-client-1.8.0.tar", last modified: Sat Sep 21 10:23:44 2019, max compression
+gzip compressed data, was "dist/cloudfoundry-client-1.9.0.tar", last modified: Fri Sep 27 12:26:23 2019, max compression
```

## Comparing `cloudfoundry-client-1.8.0.tar` & `cloudfoundry-client-1.9.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)       38 2016-11-09 14:48:56.000000 cloudfoundry-client-1.8.0/MANIFEST.in
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      104 2019-09-21 10:22:39.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/__init__.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/__init__.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    10746 2019-03-13 09:36:18.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/main.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     8401 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/command_domain.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2818 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/tasks_command_domain.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     4368 2018-11-20 07:09:54.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/apps_command_domain.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      828 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/operation_commands.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10224 2019-09-21 08:09:35.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/client.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      404 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/resources.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2016-11-09 14:48:56.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/__init__.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      327 2019-09-21 10:16:19.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/events.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      594 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_plans.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     1120 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_brokers.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      356 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/jobs.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      831 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/routes.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     6660 2019-09-21 10:21:10.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/entities.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      595 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_keys.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      657 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_bindings.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     1958 2019-05-28 18:28:43.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_instances.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     7680 2019-07-10 16:06:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/apps.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      370 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/buildpacks.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/__init__.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     5781 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/entities.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      319 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/apps.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      791 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/tasks.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/__init__.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2919 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/error_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     5108 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/log_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    12046 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/envelope_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2450 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/uuid_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     8860 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/metric_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    16311 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/http_pb2.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      495 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/errors.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      159 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/json_object.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/__init__.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/__init__.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    18542 2019-07-11 08:50:07.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/push.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     2038 2019-07-10 15:23:55.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/file_helper.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/validation/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/validation/__init__.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     5991 2019-07-10 16:04:58.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/validation/manifest.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     1547 2019-07-11 11:25:09.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/cf_ignore.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      804 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/imported.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      146 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/request_object.py
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/__init__.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     4355 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/client.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     1265 2018-11-19 21:40:59.000000 cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/websocket_envelope_reader.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2888 2018-11-19 21:42:33.000000 cloudfoundry-client-1.8.0/setup.py
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10603 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/PKG-INFO
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)       59 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/setup.cfg
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     7749 2019-09-21 10:22:12.000000 cloudfoundry-client-1.8.0/README.rst
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)        1 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/dependency_links.txt
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)        1 2019-05-28 18:31:34.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/zip-safe
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)       76 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/entry_points.txt
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)       20 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/top_level.txt
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10603 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/PKG-INFO
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)       74 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/requires.txt
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)     2478 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/SOURCES.txt
-drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-21 10:23:44.000000 cloudfoundry-client-1.8.0/test/
--rw-r--r--   0 buce8373  (1000) buce8373  (1000)      563 2019-01-27 15:03:33.000000 cloudfoundry-client-1.8.0/test/test_request_object.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     6622 2018-12-13 16:52:20.000000 cloudfoundry-client-1.8.0/test/test_client.py
--rw-rw-r--   0 buce8373  (1000) buce8373  (1000)       74 2019-03-27 13:43:24.000000 cloudfoundry-client-1.8.0/requirements.txt
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)       38 2016-11-09 14:48:56.000000 cloudfoundry-client-1.9.0/MANIFEST.in
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/main/
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      104 2019-09-27 12:25:25.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/__init__.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/__init__.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    10746 2019-03-13 09:36:18.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/main.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     8401 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/command_domain.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2818 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/tasks_command_domain.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     4368 2018-11-20 07:09:54.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/apps_command_domain.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      828 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/operation_commands.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10224 2019-09-21 08:09:35.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/client.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      404 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/resources.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2016-11-09 14:48:56.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/__init__.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      327 2019-09-21 10:16:19.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/events.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      594 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_plans.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     1120 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_brokers.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      356 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/jobs.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      831 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/routes.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     6817 2019-09-27 12:25:01.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/entities.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      595 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_keys.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      657 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_bindings.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     1958 2019-05-28 18:28:43.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_instances.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     7680 2019-07-10 16:06:44.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/apps.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      370 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/buildpacks.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/__init__.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     5799 2019-09-27 12:25:01.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/entities.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      319 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/apps.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      791 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/tasks.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/__init__.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2919 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/error_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     5108 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/log_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    12046 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/envelope_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2450 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/uuid_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     8860 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/metric_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    16311 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/http_pb2.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      740 2019-09-27 12:25:01.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/errors.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      159 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/json_object.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/__init__.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/__init__.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)    18542 2019-07-11 08:50:07.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/push.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     2038 2019-07-10 15:23:55.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/file_helper.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/validation/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/validation/__init__.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     5991 2019-07-10 16:04:58.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/validation/manifest.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     1547 2019-07-11 11:25:09.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/cf_ignore.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)      804 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/imported.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      146 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/request_object.py
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)        0 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/__init__.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     4355 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/client.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     1265 2018-11-19 21:40:59.000000 cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/websocket_envelope_reader.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     2888 2018-11-19 21:42:33.000000 cloudfoundry-client-1.9.0/setup.py
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10603 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/PKG-INFO
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)       59 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/setup.cfg
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     7749 2019-09-21 10:22:12.000000 cloudfoundry-client-1.9.0/README.rst
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)        1 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/dependency_links.txt
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)        1 2019-05-28 18:31:34.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/zip-safe
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)       76 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/entry_points.txt
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)       20 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/top_level.txt
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)    10603 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/PKG-INFO
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)       74 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/requires.txt
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)     2478 2019-09-27 12:26:22.000000 cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/SOURCES.txt
+drwxr-xr-x   0 buce8373  (1000) buce8373  (1000)        0 2019-09-27 12:26:23.000000 cloudfoundry-client-1.9.0/test/
+-rw-r--r--   0 buce8373  (1000) buce8373  (1000)      563 2019-01-27 15:03:33.000000 cloudfoundry-client-1.9.0/test/test_request_object.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)     6622 2018-12-13 16:52:20.000000 cloudfoundry-client-1.9.0/test/test_client.py
+-rw-rw-r--   0 buce8373  (1000) buce8373  (1000)       74 2019-03-27 13:43:24.000000 cloudfoundry-client-1.9.0/requirements.txt
```

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/main.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/main.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/command_domain.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/command_domain.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/tasks_command_domain.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/tasks_command_domain.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/apps_command_domain.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/apps_command_domain.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/main/operation_commands.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/main/operation_commands.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/client.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_plans.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_plans.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_brokers.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_brokers.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/routes.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/routes.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/entities.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import functools
 import logging
 
+from cloudfoundry_client.errors import InvalidEntity
 from cloudfoundry_client.imported import quote, reduce
 from cloudfoundry_client.json_object import JsonObject
 from cloudfoundry_client.request_object import Request
 
 _logger = logging.getLogger(__name__)
 
 
 class Entity(JsonObject):
     def __init__(self, target_endpoint, client, *args, **kwargs):
         super(Entity, self).__init__(*args, **kwargs)
         self.target_endpoint = target_endpoint
         self.client = client
         try:
+            if 'entity' not in self:
+                raise InvalidEntity(**self)
+
             for attribute, value in list(self['entity'].items()):
                 domain_name, suffix = attribute.rpartition('_')[::2]
                 if suffix == 'url':
                     manager_name = domain_name if domain_name.endswith('s') else '%ss' % domain_name
                     try:
                         other_manager = getattr(client.v2, manager_name)
                     except AttributeError:
@@ -30,15 +34,15 @@
                     if domain_name.endswith('s'):
                         new_method = functools.partial(other_manager._list, value)
                     else:
                         new_method = functools.partial(other_manager._get, value)
                     new_method.__name__ = domain_name
                     setattr(self, domain_name, new_method)
         except KeyError:
-            raise
+            raise InvalidEntity(**self)
 
 
 class EntityManager(object):
     list_query_parameters = ['page', 'results-per-page', 'order-direction']
 
     list_multi_parameters = ['order-by']
```

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_keys.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_keys.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_bindings.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_bindings.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/service_instances.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/service_instances.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v2/apps.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v2/apps.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/entities.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import logging
 import functools
+
+from cloudfoundry_client.errors import InvalidEntity
 from cloudfoundry_client.imported import quote, reduce
 from cloudfoundry_client.json_object import JsonObject
 from cloudfoundry_client.request_object import Request
 
 _logger = logging.getLogger(__name__)
 
 
 class Entity(JsonObject):
-    def __init__(self, client, entity_manager, *args, **kwargs):
+    def __init__(self, entity_manager, *args, **kwargs):
         super(Entity, self).__init__(*args, **kwargs)
         try:
             def default_method(m, u):
                 raise NotImplementedError('Unknown method %s for url %s' % (m, u))
 
             for link_name, link in self.get('links', {}).items():
                 if link_name != 'self':
                     link_method = link.get('method', 'GET').lower()
-                    new_method = None
                     ref = link['href']
-                    if link_method== 'get':
+                    if link_method == 'get':
                         new_method = functools.partial(entity_manager._paginate, ref) if link_name.endswith('s')\
                             else functools.partial(entity_manager._get, ref)
                     elif link_method == 'post':
                         new_method = functools.partial(entity_manager._post, ref)
                     elif link_method == 'put':
                         new_method = functools.partial(entity_manager._put, ref)
                     elif link_method == 'delete':
                         new_method = functools.partial(entity_manager._delete, ref)
                     else:
                         new_method = functools.partial(default_method, link_method, ref)
                     new_method.__name__ = link_name
                     setattr(self, link_name, new_method)
         except KeyError:
-            raise
+            raise InvalidEntity(**self)
 
 
 class EntityManager(object):
     def __init__(self, target_endpoint, client, entity_uri):
         self.target_endpoint = target_endpoint
         self.entity_uri = entity_uri
         self.client = client
@@ -121,15 +122,15 @@
 
     @staticmethod
     def _request(**mandatory_parameters):
         return Request(**mandatory_parameters)
 
     def _entity(self, result):
         if 'guid' in result:
-            return Entity(self.client, self, **result)
+            return Entity(self, **result)
         else:
             return result
 
     @staticmethod
     def _get_url_filtered(url, **kwargs):
         def _append_encoded_parameter(parameters, args):
             parameter_name, parameter_value = args[0], args[1]
```

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/v3/tasks.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/v3/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/error_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/error_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/log_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/log_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/envelope_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/envelope_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/uuid_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/uuid_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/metric_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/dropsonde/http_pb2.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/dropsonde/http_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/push.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/push.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/file_helper.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/file_helper.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/validation/manifest.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/operations/push/cf_ignore.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/operations/push/cf_ignore.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/imported.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/imported.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/client.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/client.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/main/cloudfoundry_client/doppler/websocket_envelope_reader.py` & `cloudfoundry-client-1.9.0/main/cloudfoundry_client/doppler/websocket_envelope_reader.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/setup.py` & `cloudfoundry-client-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/PKG-INFO` & `cloudfoundry-client-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudfoundry-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: A client library for CloudFoundry
 Home-page: http://github.com/antechrestos/cf-python-client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Description: Cloudfoundry python client
         ==========================
```

### Comparing `cloudfoundry-client-1.8.0/README.rst` & `cloudfoundry-client-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/PKG-INFO` & `cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudfoundry-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: A client library for CloudFoundry
 Home-page: http://github.com/antechrestos/cf-python-client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Description: Cloudfoundry python client
         ==========================
```

### Comparing `cloudfoundry-client-1.8.0/cloudfoundry_client.egg-info/SOURCES.txt` & `cloudfoundry-client-1.9.0/cloudfoundry_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/test/test_request_object.py` & `cloudfoundry-client-1.9.0/test/test_request_object.py`

 * *Files identical despite different names*

### Comparing `cloudfoundry-client-1.8.0/test/test_client.py` & `cloudfoundry-client-1.9.0/test/test_client.py`

 * *Files identical despite different names*

