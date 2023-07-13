# Comparing `tmp/quao-0.3.6.tar.gz` & `tmp/quao-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.3.6.tar", last modified: Thu Jul 13 01:58:51 2023, max compression
+gzip compressed data, was "quao-0.3.7.tar", last modified: Thu Jul 13 06:54:39 2023, max compression
```

## Comparing `quao-0.3.6.tar` & `quao-0.3.7.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.119566 quao-0.3.6/
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-13 01:58:27.000000 quao-0.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-13 01:58:51.119566 quao-0.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-13 01:58:27.000000 quao-0.3.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-13 01:58:27.000000 quao-0.3.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 01:58:51.119566 quao-0.3.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.099566 quao-0.3.6/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/config/logging_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao/data/job/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/data/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/data/job/job_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao/data/request/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/data/request/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/data/request/request_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.107566 quao-0.3.6/src/quao/enum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/http_header.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/http_status.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/job_status.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/media_type.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/processing_unit.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/provider_type.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/enum/token_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.111566 quao-0.3.6/src/quao/factory/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/factory/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/factory/device_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/factory/provider_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.111566 quao-0.3.6/src/quao/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.115566 quao-0.3.6/src/quao/model/device/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2391 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/device.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/device/quao_device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.115566 quao-0.3.6/src/quao/model/job/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/job/qiskit_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.119566 quao-0.3.6/src/quao/model/provider/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      968 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/model/provider/quao_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.119566 quao-0.3.6/src/quao/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/util/json_parser_util.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-13 01:58:27.000000 quao-0.3.6/src/quao/util/response_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 01:58:51.103566 quao-0.3.6/src/quao.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-13 01:58:51.000000 quao-0.3.6/src/quao.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1537 2023-07-13 01:58:51.000000 quao-0.3.6/src/quao.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 01:58:51.000000 quao-0.3.6/src/quao.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      201 2023-07-13 01:58:51.000000 quao-0.3.6/src/quao.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-13 01:58:51.000000 quao-0.3.6/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.710823 quao-0.3.7/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-07-13 06:54:39.709809 quao-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.7/README.md
+-rw-rw-rw-   0        0        0      967 2023-07-13 04:05:15.000000 quao-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 06:54:39.710823 quao-0.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.466284 quao-0.3.7/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.485071 quao-0.3.7/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-07-13 04:05:56.000000 quao-0.3.7/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     7544 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.512740 quao-0.3.7/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.7/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.7/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.513709 quao-0.3.7/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.521710 quao-0.3.7/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.7/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.528713 quao-0.3.7/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.7/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.581505 quao-0.3.7/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.7/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.7/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.7/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.7/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.598514 quao-0.3.7/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.7/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.7/src/quao/factory/provider_factory.py
+-rw-rw-rw-   0        0        0      691 2023-07-13 04:03:48.000000 quao-0.3.7/src/quao/invocation_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.599515 quao-0.3.7/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.647591 quao-0.3.7/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2463 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3612 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.7/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      788 2023-07-12 04:24:43.000000 quao-0.3.7/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1170 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3337 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.655819 quao-0.3.7/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     3938 2023-07-13 04:03:03.000000 quao-0.3.7/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.690812 quao-0.3.7/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.7/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.7/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.7/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.7/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.7/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.708810 quao-0.3.7/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.7/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.7/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.7/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:54:39.505710 quao-0.3.7/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-07-13 06:54:39.000000 quao-0.3.7/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2023-07-13 06:54:39.000000 quao-0.3.7/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:54:39.000000 quao-0.3.7/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      201 2023-07-13 06:54:39.000000 quao-0.3.7/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 06:54:39.000000 quao-0.3.7/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.3.6/LICENSE` & `quao-0.3.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-The MIT License (MIT)
-Copyright © CITYNOW Co. Ltd. All rights reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+The MIT License (MIT)
+Copyright © CITYNOW Co. Ltd. All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `quao-0.3.6/PKG-INFO` & `quao-0.3.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: quao
-Version: 0.3.6
-Summary: Quao Library supporting Quao Platform for Quantum Computing
-Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
-License: The MIT License (MIT)
-        Copyright © CITYNOW Co. Ltd. All rights reserved.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://citynow.vn/
-Keywords: quao,quantum
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+Metadata-Version: 2.1
+Name: quao
+Version: 0.3.7
+Summary: Quao Library supporting Quao Platform for Quantum Computing
+Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
+License: The MIT License (MIT)
+        Copyright © CITYNOW Co. Ltd. All rights reserved.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://citynow.vn/
+Keywords: quao,quantum
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.3.6/README.md` & `quao-0.3.7/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.3.6/pyproject.toml` & `quao-0.3.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "quao"
-version = "0.3.6"
-description = "Quao Library supporting Quao Platform for Quantum Computing"
-readme = "README.md"
-authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["quao", "quantum"]
-dependencies = [
-    "qiskit==0.42.1",
-    "qiskit-aer==0.12.0",
-    "qiskit-aer-gpu",
-    "qbraid==0.4.0",
-    "amazon-braket-sdk==1.38.1",
-    "qiskit-ibm-runtime",
-    "qiskit-ibm-provider",
-    "matplotlib",
-    "pylatexenc",
-    "loguru"
-]
-requires-python = ">=3.7"
-
-[project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
-
-[project.urls]
-Homepage = "https://citynow.vn/"
-
+
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "quao"
+version = "0.3.7"
+description = "Quao Library supporting Quao Platform for Quantum Computing"
+readme = "README.md"
+authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["quao", "quantum"]
+dependencies = [
+    "qiskit==0.42.1",
+    "qiskit-aer==0.12.0",
+    "qiskit-aer-gpu",
+    "qbraid==0.4.0",
+    "amazon-braket-sdk==1.38.1",
+    "qiskit-ibm-runtime",
+    "qiskit-ibm-provider",
+    "matplotlib",
+    "pylatexenc",
+    "loguru"
+]
+requires-python = ">=3.7"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+
+[project.urls]
+Homepage = "https://citynow.vn/"
+
```

### Comparing `quao-0.3.6/src/quao/backend.py` & `quao-0.3.7/src/quao/backend.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-"""
-    QuaO Project backend.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-import io
-from json import JSONDecodeError
-
-import requests
-from braket.circuits import Circuit
-from qbraid import circuit_wrapper
-from qiskit import transpile, Aer
-from qiskit_ibm_provider import IBMProvider
-
-from .data.job.job_response import JobResponse
-from .data.request.request_data import RequestData
-from .enum.http_header import HttpHeader
-from .enum.job_status import JobStatus
-from .enum.media_type import MediaType
-from .enum.provider_type import ProviderType
-from .enum.sdk import Sdk
-from .enum.token_type import TokenType
-from .factory.device_factory import DeviceFactory
-from .factory.provider_factory import ProviderFactory
-from .config.logging_config import *
-
-
-class Backend:
-    def __init__(self, request_data: RequestData):
-        self.server_url = request_data.server_url
-        self.sdk = request_data.sdk
-        self.input = request_data.input
-        self.shots = request_data.shots
-        self.circuit_export_url = request_data.circuit_export_url
-        self.device_id = request_data.device_id
-        self.backend_data = None
-        self.user_token = request_data.user_token
-        self.user_identity = request_data.user_identity
-
-    def submit_job(self, circuit) -> JobResponse:
-        """
-
-        @param circuit:
-        @return:
-        """
-        logger.debug('Pre-execute job!')
-        self.__pre_execute_job(circuit)
-
-        logger.debug('Execute job!')
-        job_response = self.__execute_job(circuit)
-
-        logger.debug('Post-execute job!')
-        self.__post_execute_job(circuit)
-
-        return job_response
-
-    @staticmethod
-    def __get_qubit_number(circuit, sdk) -> int:
-        """
-
-        @param circuit:
-        @param sdk:
-        @return:
-        """
-
-        if Sdk.QISKIT.value.__eq__(sdk):
-            return int(circuit.num_qubits)
-
-        if Sdk.BRAKET.value.__eq__(sdk):
-            return circuit.qubit_count
-
-        return 0
-
-    @staticmethod
-    def __generate_backend_request(device_id, required_qubit):
-        """
-
-        @param device_id:
-        @param required_qubit:
-        @return:
-        """
-
-        backend_request = {
-            "deviceId": device_id,
-            "qubitAmount": required_qubit
-        }
-
-        return backend_request
-
-    @staticmethod
-    def __generate_backend_header(user_token):
-        """
-
-        @param user_token:
-        """
-        backend_header = {
-            HttpHeader.AUTHORIZATION.value: TokenType.BEARER.value + ' ' + user_token
-        }
-
-        return backend_header
-
-    def __set_backend_data(self, backend_request, backend_header):
-        """
-
-        @param backend_request:
-        """
-
-        response = requests.get(
-            self.server_url,
-            params=backend_request,
-            headers=backend_header
-        )
-        if response.status_code == 200:
-            try:
-                self.backend_data = response.json().get("data")
-            except JSONDecodeError:
-                pass
-        else:
-            pass
-
-    def __pre_execute_job(self, circuit):
-        """
-
-        @param circuit:
-        """
-
-        required_qubit = self.__get_qubit_number(circuit, self.sdk)
-        backend_request = self.__generate_backend_request(self.device_id, required_qubit)
-        backend_header = self.__generate_backend_header(self.user_token)
-
-        logger.debug('Device selection request: {0}'.format(backend_request))
-
-        self.__set_backend_data(backend_request, backend_header)
-
-    def __execute_job(self, circuit) -> JobResponse:
-        """
-
-        @param circuit:
-        @return:
-        """
-
-        error_job_response = JobResponse()
-        error_job_response.job_status = JobStatus.ERROR.value
-        error_job_response.user_identity = self.user_identity
-        error_job_response.user_token = self.user_token
-
-        shots = self.shots
-
-        if circuit and self.backend_data:
-            device_name = self.backend_data.get("deviceName")
-            provider_tag = self.backend_data.get("providerTag")
-            authentication = self.backend_data.get("authentication")
-
-            try:
-                logger.debug('Execute job with provider tag: {0}'.format(provider_tag))
-                provider = ProviderFactory().create_provider(provider_tag, authentication)
-
-                logger.debug('Execute job with device name: {0}'.format(device_name))
-                device = DeviceFactory().create_device(provider, device_name, authentication,
-                                                       self.sdk)
-
-                job_response = device.run_circuit(circuit=circuit, shots=shots)
-                job_response.user_identity = self.user_identity
-                job_response.user_token = self.user_token
-
-                return job_response
-
-            except Exception as exception:
-                error_job_response.job_result = {"error": str(exception)}
-
-        elif self.backend_data is None:
-            error_job_response.job_result = {"error": "Backend not found"}
-
-        return error_job_response
-
-    def __post_execute_job(self, circuit):
-        """
-
-        @param circuit:
-        """
-
-        self.__export_circuit(circuit)
-
-    def __export_circuit(self, circuit):
-        """
-          Export circuit to svg file then send to QuaO server for saving
-          Args:
-              circuit: circuit will be exported
-              @param circuit:
-        """
-        if self.circuit_export_url is None or len(self.circuit_export_url) < 1:
-            return
-
-        logger.debug("Preparing circuit figure...")
-        transpiled_circuit = self.__transpile_circuit(circuit)
-        circuit_figure = transpiled_circuit.draw(output='mpl', fold=-1)
-
-        logger.debug("Converting circuit figure to svg file...")
-        figure_buffer = io.BytesIO()
-        circuit_figure.savefig(figure_buffer, format='svg', bbox_inches='tight')
-
-        logger.debug("Sending circuit svg image to [{0}] with POST method ...".format(
-            self.circuit_export_url))
-
-        payload = {'circuit': (
-            'circuit_figure',
-            figure_buffer.getvalue(),
-            MediaType.MULTIPART_FORM_DATA.value)}
-
-        response = requests.post(url=self.circuit_export_url,
-                                 headers=self.__generate_backend_header(self.user_token),
-                                 files=payload)
-        if response.ok:
-            logger.debug("Sending request to QuaO backend successfully!")
-        else:
-            logger.debug("Sending request to QuaO backend failed with status {0}!".format(
-                response.status_code))
-
-    def __transpile_circuit(self, circuit):
-        if isinstance(circuit, Circuit):
-            return circuit_wrapper(circuit).transpile(Sdk.QISKIT.value)
-
-        qiskit_device_name = self.backend_data.get("deviceName")
-
-        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(self.backend_data.get("providerTag")):
-            return transpile(circuits=circuit,
-                             backend=Aer.get_backend(qiskit_device_name))
-
-        provider = IBMProvider(token=self.backend_data.get("authentication").get('token'))
-        backend = provider.get_backend(qiskit_device_name)
-
-        return transpile(circuits=circuit, backend=backend)
+"""
+    QuaO Project backend.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+import io
+from json import JSONDecodeError
+
+import requests
+from braket.circuits import Circuit
+from qbraid import circuit_wrapper
+from qiskit import transpile, Aer
+from qiskit_ibm_provider import IBMProvider
+
+from .data.job.job_response import JobResponse
+from .data.request.request_data import RequestData
+from .enum.http_header import HttpHeader
+from .enum.job_status import JobStatus
+from .enum.media_type import MediaType
+from .enum.provider_type import ProviderType
+from .enum.sdk import Sdk
+from .enum.token_type import TokenType
+from .factory.device_factory import DeviceFactory
+from .factory.provider_factory import ProviderFactory
+from .config.logging_config import *
+
+
+class Backend:
+    def __init__(self, request_data: RequestData):
+        self.server_url = request_data.server_url
+        self.sdk = request_data.sdk
+        self.input = request_data.input
+        self.shots = request_data.shots
+        self.circuit_export_url = request_data.circuit_export_url
+        self.device_id = request_data.device_id
+        self.backend_data = None
+        self.user_token = request_data.user_token
+        self.user_identity = request_data.user_identity
+
+    def submit_job(self, circuit) -> JobResponse:
+        """
+
+        @param circuit:
+        @return:
+        """
+        logger.debug('Pre-execute job!')
+        self.__pre_execute_job(circuit)
+
+        logger.debug('Execute job!')
+        job_response = self.__execute_job(circuit)
+
+        logger.debug('Post-execute job!')
+        self.__post_execute_job(circuit)
+
+        return job_response
+
+    @staticmethod
+    def __get_qubit_number(circuit, sdk) -> int:
+        """
+
+        @param circuit:
+        @param sdk:
+        @return:
+        """
+
+        if Sdk.QISKIT.value.__eq__(sdk):
+            return int(circuit.num_qubits)
+
+        if Sdk.BRAKET.value.__eq__(sdk):
+            return circuit.qubit_count
+
+        return 0
+
+    @staticmethod
+    def __generate_backend_request(device_id, required_qubit):
+        """
+
+        @param device_id:
+        @param required_qubit:
+        @return:
+        """
+
+        backend_request = {
+            "deviceId": device_id,
+            "qubitAmount": required_qubit
+        }
+
+        return backend_request
+
+    @staticmethod
+    def __generate_backend_header(user_token):
+        """
+
+        @param user_token:
+        """
+        backend_header = {
+            HttpHeader.AUTHORIZATION.value: TokenType.BEARER.value + ' ' + user_token
+        }
+
+        return backend_header
+
+    def __set_backend_data(self, backend_request, backend_header):
+        """
+
+        @param backend_request:
+        """
+
+        response = requests.get(
+            self.server_url,
+            params=backend_request,
+            headers=backend_header
+        )
+        if response.status_code == 200:
+            try:
+                self.backend_data = response.json().get("data")
+            except JSONDecodeError:
+                pass
+        else:
+            pass
+
+    def __pre_execute_job(self, circuit):
+        """
+
+        @param circuit:
+        """
+
+        required_qubit = self.__get_qubit_number(circuit, self.sdk)
+        backend_request = self.__generate_backend_request(self.device_id, required_qubit)
+        backend_header = self.__generate_backend_header(self.user_token)
+
+        logger.debug('Device selection request: {0}'.format(backend_request))
+
+        self.__set_backend_data(backend_request, backend_header)
+
+    def __execute_job(self, circuit) -> JobResponse:
+        """
+
+        @param circuit:
+        @return:
+        """
+
+        error_job_response = JobResponse()
+        error_job_response.job_status = JobStatus.ERROR.value
+        error_job_response.user_identity = self.user_identity
+        error_job_response.user_token = self.user_token
+
+        shots = self.shots
+
+        if circuit and self.backend_data:
+            device_name = self.backend_data.get("deviceName")
+            provider_tag = self.backend_data.get("providerTag")
+            authentication = self.backend_data.get("authentication")
+
+            try:
+                logger.debug('Execute job with provider tag: {0}'.format(provider_tag))
+                provider = ProviderFactory().create_provider(provider_tag, authentication)
+
+                logger.debug('Execute job with device name: {0}'.format(device_name))
+                device = DeviceFactory().create_device(provider, device_name, authentication,
+                                                       self.sdk)
+
+                job_response = device.run_circuit(circuit=circuit, shots=shots)
+                job_response.user_identity = self.user_identity
+                job_response.user_token = self.user_token
+
+                return job_response
+
+            except Exception as exception:
+                error_job_response.job_result = {"error": str(exception)}
+
+        elif self.backend_data is None:
+            error_job_response.job_result = {"error": "Backend not found"}
+
+        return error_job_response
+
+    def __post_execute_job(self, circuit):
+        """
+
+        @param circuit:
+        """
+
+        self.__export_circuit(circuit)
+
+    def __export_circuit(self, circuit):
+        """
+          Export circuit to svg file then send to QuaO server for saving
+          Args:
+              circuit: circuit will be exported
+              @param circuit:
+        """
+        if self.circuit_export_url is None or len(self.circuit_export_url) < 1:
+            return
+
+        logger.debug("Preparing circuit figure...")
+        transpiled_circuit = self.__transpile_circuit(circuit)
+        circuit_figure = transpiled_circuit.draw(output='mpl', fold=-1)
+
+        logger.debug("Converting circuit figure to svg file...")
+        figure_buffer = io.BytesIO()
+        circuit_figure.savefig(figure_buffer, format='svg', bbox_inches='tight')
+
+        logger.debug("Sending circuit svg image to [{0}] with POST method ...".format(
+            self.circuit_export_url))
+
+        payload = {'circuit': (
+            'circuit_figure',
+            figure_buffer.getvalue(),
+            MediaType.MULTIPART_FORM_DATA.value)}
+
+        response = requests.post(url=self.circuit_export_url,
+                                 headers=self.__generate_backend_header(self.user_token),
+                                 files=payload)
+        if response.ok:
+            logger.debug("Sending request to QuaO backend successfully!")
+        else:
+            logger.debug("Sending request to QuaO backend failed with status {0}!".format(
+                response.status_code))
+
+    def __transpile_circuit(self, circuit):
+        if isinstance(circuit, Circuit):
+            return circuit_wrapper(circuit).transpile(Sdk.QISKIT.value)
+
+        qiskit_device_name = self.backend_data.get("deviceName")
+
+        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(self.backend_data.get("providerTag")):
+            return transpile(circuits=circuit,
+                             backend=Aer.get_backend(qiskit_device_name))
+
+        provider = IBMProvider(token=self.backend_data.get("authentication").get('token'))
+        backend = provider.get_backend(qiskit_device_name)
+
+        return transpile(circuits=circuit, backend=backend)
```

### Comparing `quao-0.3.6/src/quao/data/job/job_response.py` & `quao-0.3.7/src/quao/data/job/job_response.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-    QuaO Project job_response.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from ...enum.media_type import MediaType
-from ...enum.job_status import JobStatus
-
-
-class JobResponse(object):
-    def __init__(
-            self,
-            provider_job_id: str = "",
-            job_status: str = "",
-            job_result=None,
-            content_type=None,
-            job_histogram=None,
-            user_identity="",
-            user_token="",
-            execution_time=None
-    ):
-        self.provider_job_id = provider_job_id if provider_job_id else ""
-        self.job_status = job_status if job_status else JobStatus.ERROR.value
-        self.job_result = job_result
-        self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
-        self.job_histogram = job_histogram
-        self.user_identity = user_identity
-        self.user_token = user_token
-        self.execution_time = execution_time
+"""
+    QuaO Project job_response.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from ...enum.media_type import MediaType
+from ...enum.job_status import JobStatus
+
+
+class JobResponse(object):
+    def __init__(
+            self,
+            provider_job_id: str = "",
+            job_status: str = "",
+            job_result=None,
+            content_type=None,
+            job_histogram=None,
+            user_identity="",
+            user_token="",
+            execution_time=None
+    ):
+        self.provider_job_id = provider_job_id if provider_job_id else ""
+        self.job_status = job_status if job_status else JobStatus.ERROR.value
+        self.job_result = job_result
+        self.content_type = content_type if content_type else MediaType.ALL_TYPE.value
+        self.job_histogram = job_histogram
+        self.user_identity = user_identity
+        self.user_token = user_token
+        self.execution_time = execution_time
```

### Comparing `quao-0.3.6/src/quao/data/request/request_data.py` & `quao-0.3.7/src/quao/data/request/request_data.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-    QuaO Project request_data.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-
-
-class RequestData:
-
-    def __init__(self, event):
-        json_data = event.json()
-        self.data = json_data
-        self.input = json_data.get("input")
-        self.shots = json_data.get("shots")
-        self.device_id = json_data.get("deviceId")
-        self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
-        self.server_url = json_data.get("serverUrl")
-        self.circuit_export_url = json_data.get("circuitExportUrl")
-        self.user_token = json_data.get("userToken")
-        self.user_identity = json_data.get("userIdentity")
+"""
+    QuaO Project request_data.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+
+
+class RequestData:
+
+    def __init__(self, event):
+        json_data = event.json()
+        self.data = json_data
+        self.input = json_data.get("input")
+        self.shots = json_data.get("shots")
+        self.device_id = json_data.get("deviceId")
+        self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
+        self.server_url = json_data.get("serverUrl")
+        self.circuit_export_url = json_data.get("circuitExportUrl")
+        self.user_token = json_data.get("userToken")
+        self.user_identity = json_data.get("userIdentity")
```

### Comparing `quao-0.3.6/src/quao/factory/provider_factory.py` & `quao-0.3.7/src/quao/factory/provider_factory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-    QuaO Project provider_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from ..enum.provider_type import ProviderType
-from ..model.provider.aws_braket_provider import AwsBraketProvider
-from ..model.provider.ibm_cloud_provider import IbmCloudProvider
-from ..model.provider.ibm_quantum_provider import IbmQuantumProvider
-from ..model.provider.quao_provider import QuaoProvider
-
-
-class ProviderFactory:
-
-    @staticmethod
-    def create_provider(provider_type: str, authentication: dict):
-        """
-
-        @param provider_type:
-        @param authentication:
-        @return:
-        """
-
-        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
-            return QuaoProvider()
-
-        if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
-            return IbmQuantumProvider(authentication.get('token'))
-
-        if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
-            return IbmCloudProvider(authentication.get('token'), authentication.get('crn'))
-
-        if ProviderType.AWS_BRAKET.value.__eq__(provider_type):
-            return AwsBraketProvider(
-                authentication.get('accessKey'),
-                authentication.get('secretKey'),
-                authentication.get('regionName'))
-
-        raise Exception("Unsupported provider!")
+"""
+    QuaO Project provider_factory.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from ..enum.provider_type import ProviderType
+from ..model.provider.aws_braket_provider import AwsBraketProvider
+from ..model.provider.ibm_cloud_provider import IbmCloudProvider
+from ..model.provider.ibm_quantum_provider import IbmQuantumProvider
+from ..model.provider.quao_provider import QuaoProvider
+
+
+class ProviderFactory:
+
+    @staticmethod
+    def create_provider(provider_type: str, authentication: dict):
+        """
+
+        @param provider_type:
+        @param authentication:
+        @return:
+        """
+
+        if ProviderType.QUAO_QUANTUM_SIMULATOR.value.__eq__(provider_type):
+            return QuaoProvider()
+
+        if ProviderType.IBM_QUANTUM.value.__eq__(provider_type):
+            return IbmQuantumProvider(authentication.get('token'))
+
+        if ProviderType.IBM_CLOUD.value.__eq__(provider_type):
+            return IbmCloudProvider(authentication.get('token'), authentication.get('crn'))
+
+        if ProviderType.AWS_BRAKET.value.__eq__(provider_type):
+            return AwsBraketProvider(
+                authentication.get('accessKey'),
+                authentication.get('secretKey'),
+                authentication.get('regionName'))
+
+        raise Exception("Unsupported provider!")
```

### Comparing `quao-0.3.6/src/quao/model/device/aws_braket_device.py` & `quao-0.3.7/src/quao/model/device/aws_braket_device.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-"""
-    QuaO Project aws_braket_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from ..device.device import Device
-from ..provider.provider import Provider
-from ...enum.job_status import JobStatus
-from ...util.json_parser_util import JsonParserUtils
-from ...config.logging_config import *
-from dateutil.parser import parse
-
-
-class AwsBraketDevice(Device):
-    def _get_name(self) -> str:
-        return str(self.device.name)
-
-    def __init__(self, provider: Provider,
-                 device_specification: str,
-                 s3_bucket_name: str,
-                 s3_prefix: str):
-        super().__init__(provider, device_specification)
-        self.s3_folder = (s3_bucket_name, s3_prefix)
-
-    def _create_job(self, circuit, shots):
-        logger.debug('Create AWS Braket job with {0} shots'.format(shots))
-
-        job = self.device.run(task_specification=circuit,
-                              s3_destination_folder=self.s3_folder,
-                              shots=shots)
-        return job
-
-    def _is_simulator(self) -> bool:
-        return 'SIMULATOR'.__eq__(self.device.type.value)
-
-    def _produce_histogram_data(self, job_result) -> dict:
-        return dict(job_result.measurement_counts)
-
-    def _get_provider_job_id(self, job) -> str:
-        return job.id
-
-    def _get_job_status(self, job) -> str:
-        job_state = job.state()
-        if JobStatus.COMPLETED.value.__eq__(job_state):
-            job_state = JobStatus.DONE.value
-        return job_state
-
-    def _parse_job_result(self, job_result) -> dict:
-        return JsonParserUtils.parse(job_result.__dict__)
-
-    def _calculate_execution_time(self, job_result):
-        if 'task_metadata' not in job_result:
-            return
-
-        task_metadata = job_result['task_metadata']
-
-        if task_metadata is None \
-                or not bool(task_metadata)\
-                or 'createdAt' not in task_metadata \
-                or 'endedAt' not in task_metadata:
-            return
-
-        created_at = task_metadata['createdAt']
-        ended_at = task_metadata['endedAt']
-
-        if created_at is None or ended_at is None:
-            return
-
-        created_at = parse(created_at.replace("T", " ").replace("Z", ""))
-        ended_at = parse(ended_at.replace("T", " ").replace("Z", ""))
-
-        offset = ended_at - created_at
-
-        self.execution_time = offset.total_seconds()
+"""
+    QuaO Project aws_braket_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from ..device.device import Device
+from ..provider.provider import Provider
+from ...enum.job_status import JobStatus
+from ...util.json_parser_util import JsonParserUtils
+from ...config.logging_config import *
+from dateutil.parser import parse
+
+
+class AwsBraketDevice(Device):
+    def _get_name(self) -> str:
+        return str(self.device.name)
+
+    def __init__(self, provider: Provider,
+                 device_specification: str,
+                 s3_bucket_name: str,
+                 s3_prefix: str):
+        super().__init__(provider, device_specification)
+        self.s3_folder = (s3_bucket_name, s3_prefix)
+
+    def _create_job(self, circuit, shots):
+        logger.debug('Create AWS Braket job with {0} shots'.format(shots))
+
+        job = self.device.run(task_specification=circuit,
+                              s3_destination_folder=self.s3_folder,
+                              shots=shots)
+        return job
+
+    def _is_simulator(self) -> bool:
+        return 'SIMULATOR'.__eq__(self.device.type.value)
+
+    def _produce_histogram_data(self, job_result) -> dict:
+        return dict(job_result.measurement_counts)
+
+    def _get_provider_job_id(self, job) -> str:
+        return job.id
+
+    def _get_job_status(self, job) -> str:
+        job_state = job.state()
+        if JobStatus.COMPLETED.value.__eq__(job_state):
+            job_state = JobStatus.DONE.value
+        return job_state
+
+    def _parse_job_result(self, job_result) -> dict:
+        return JsonParserUtils.parse(job_result.__dict__)
+
+    def _calculate_execution_time(self, job_result):
+        if 'task_metadata' not in job_result:
+            return
+
+        task_metadata = job_result['task_metadata']
+
+        if task_metadata is None \
+                or not bool(task_metadata)\
+                or 'createdAt' not in task_metadata \
+                or 'endedAt' not in task_metadata:
+            return
+
+        created_at = task_metadata['createdAt']
+        ended_at = task_metadata['endedAt']
+
+        if created_at is None or ended_at is None:
+            return
+
+        created_at = parse(created_at.replace("T", " ").replace("Z", ""))
+        ended_at = parse(ended_at.replace("T", " ").replace("Z", ""))
+
+        offset = ended_at - created_at
+
+        self.execution_time = offset.total_seconds()
```

### Comparing `quao-0.3.6/src/quao/model/device/ibm_quantum_device.py` & `quao-0.3.7/src/quao/model/device/ibm_quantum_device.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-    QuaO Project ibm_quantum_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-
-from qiskit import transpile
-
-from ...model.device.qiskit_device import QiskitDevice
-from ...util.json_parser_util import JsonParserUtils
-from ...config.logging_config import *
-
-
-class IbmQuantumDevice(QiskitDevice):
-
-    def _is_simulator(self) -> bool:
-        return self.device.configuration().simulator
-
-    def _parse_job_result(self, job_result) -> dict:
-        return JsonParserUtils.parse(job_result.to_dict())
-
-    def _create_job(self, circuit, shots):
-        logger.debug('Create Ibm Quantum job with {0} shots'.format(shots))
-        transpile_circuit = transpile(circuit, self.device)
-
-        return self.device.run(transpile_circuit, shots=shots)
+"""
+    QuaO Project ibm_quantum_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+
+from qiskit import transpile
+
+from ...model.device.qiskit_device import QiskitDevice
+from ...util.json_parser_util import JsonParserUtils
+from ...config.logging_config import *
+
+
+class IbmQuantumDevice(QiskitDevice):
+
+    def _is_simulator(self) -> bool:
+        return self.device.configuration().simulator
+
+    def _parse_job_result(self, job_result) -> dict:
+        return JsonParserUtils.parse(job_result.to_dict())
+
+    def _create_job(self, circuit, shots):
+        logger.debug('Create Ibm Quantum job with {0} shots'.format(shots))
+        transpile_circuit = transpile(circuit, self.device)
+
+        return self.device.run(transpile_circuit, shots=shots)
```

### Comparing `quao-0.3.6/src/quao/model/device/qiskit_device.py` & `quao-0.3.7/src/quao/model/device/qiskit_device.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-"""
-    QuaO Project qiskit_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from abc import ABC
-
-from qiskit import QiskitError
-
-from ...model.device.device import Device
-from ...config.logging_config import *
-
-
-class QiskitDevice(Device, ABC):
-
-    def _produce_histogram_data(self, job_result) -> dict:
-        try:
-            histogram_data = job_result.get_counts()
-        except QiskitError as qiskit_error:
-            logger.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
-            histogram_data = None
-
-        return histogram_data
-
-    def _get_provider_job_id(self, job) -> str:
-        return job.job_id()
-
-    def _get_job_status(self, job) -> str:
-        return job.status().name
-
-    def _get_name(self) -> str:
-        return str(self.device.configuration().backend_name)
-
-    def _calculate_execution_time(self, job_result):
-        if 'metadata' not in job_result:
-            return
-
-        metadata = job_result['metadata']
-
-        if metadata is None or not bool(metadata):
-            return
-
-        self.execution_time = metadata['time_taken_execute']
+"""
+    QuaO Project qiskit_device.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from abc import ABC
+
+from qiskit import QiskitError
+
+from ...model.device.device import Device
+from ...config.logging_config import *
+
+
+class QiskitDevice(Device, ABC):
+
+    def _produce_histogram_data(self, job_result) -> dict:
+        try:
+            histogram_data = job_result.get_counts()
+        except QiskitError as qiskit_error:
+            logger.debug("Can't produce histogram with error: {0}".format(str(qiskit_error)))
+            histogram_data = None
+
+        return histogram_data
+
+    def _get_provider_job_id(self, job) -> str:
+        return job.job_id()
+
+    def _get_job_status(self, job) -> str:
+        return job.status().name
+
+    def _get_name(self) -> str:
+        return str(self.device.configuration().backend_name)
+
+    def _calculate_execution_time(self, job_result):
+        if 'metadata' not in job_result:
+            return
+
+        metadata = job_result['metadata']
+
+        if metadata is None or not bool(metadata):
+            return
+
+        self.execution_time = metadata['time_taken_execute']
```

### Comparing `quao-0.3.6/src/quao/model/job/qiskit_status.py` & `quao-0.3.7/src/quao/model/job/qiskit_status.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-"""
-    QuaO Project job_status.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_ibm_runtime import QiskitRuntimeService
-
-from ...data.job.job_response import JobResponse
-from ...enum.job_status import JobStatus
-from ...enum.media_type import MediaType
-from ...util.json_parser_util import JsonParserUtils
-from ...config.logging_config import *
-
-
-class Job:
-    def __init__(self, channel, token, crn, provider_job_id, user_identity):
-        self.channel = channel if channel else "ibm_quantum"
-        self.token = token if token else ""
-        self.crn = crn
-        self.job_id = provider_job_id if provider_job_id else ""
-        self.retrieve_job = self.__get_job()
-        self.user_identity = user_identity
-
-    def fetch_job(self) -> JobResponse:
-        logger.info("Start get job info.")
-
-        provider_job_id = self._get_provider_job_id()
-        job_status = self._get_job_status()
-        job_result_dictionary = {}
-        content_type = None
-        job_histogram = None
-        execution_time = None
-
-        try:
-            if JobStatus.DONE.value.__eq__(job_status):
-                logger.info("Try to get job result")
-
-                job_result = self.retrieve_job.result()
-                job_status = self._get_job_status()
-
-                logger.info("Parsing job result")
-                job_result_dictionary = self._parse_job_result(job_result)
-
-                content_type = MediaType.APPLICATION_JSON.value
-
-                logger.info("Producing histogram")
-                job_histogram = self._produce_histogram_data(job_result)
-
-                logger.debug('Calculating execution time ....')
-                execution_time = self._get_execution_time(job_result_dictionary)
-                logger.debug('Execution time calculation completed!')
-
-        except Exception as exception:
-
-            logger.info("Try to job result error.")
-            job_result_dictionary = {
-                "error": "Exception when invoke job on device: " + self.retrieve_job.backend().backend_name,
-                "exception": str(exception)
-            }
-
-            job_status = JobStatus.ERROR.value
-
-        return JobResponse(
-            provider_job_id=provider_job_id,
-            job_status=job_status,
-            job_result=job_result_dictionary,
-            content_type=content_type,
-            job_histogram=job_histogram,
-            user_identity=self.user_identity,
-            execution_time=execution_time
-        )
-
-    def __get_job(self):
-        logger.info("Has IBM token: {0}".format((self.token is not None) and (len(self.token) > 0)))
-
-        service = QiskitRuntimeService(channel=self.channel,
-                                       token=self.token,
-                                       instance=self.crn)
-
-        return service.job(job_id=self.job_id)
-
-    def _get_provider_job_id(self) -> str:
-        return self.retrieve_job.job_id()
-
-    def _get_job_status(self) -> str:
-        return self.retrieve_job.status().name
-
-    @staticmethod
-    def _produce_histogram_data(job_result) -> dict:
-        try:
-            histogram_data = job_result.get_counts()
-        except Exception:
-            histogram_data = None
-
-        return histogram_data
-
-    def _parse_job_result(self, job_result):
-        if self.retrieve_job.program_id == 'sampler':
-            return JsonParserUtils.parse(job_result.__dict__)
-        return JsonParserUtils.parse(job_result.to_dict())
-
-    @staticmethod
-    def _get_execution_time(job_result):
-        if 'metadata' not in job_result:
-            return None
-
-        metadata = job_result['metadata']
-
-        if metadata is None \
-                or not bool(metadata) \
-                or 'time_taken_execute' not in metadata:
-            return None
-
-        return metadata['time_taken_execute']
+"""
+    QuaO Project job_status.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from qiskit_ibm_runtime import QiskitRuntimeService
+
+from ...data.job.job_response import JobResponse
+from ...enum.job_status import JobStatus
+from ...enum.media_type import MediaType
+from ...util.json_parser_util import JsonParserUtils
+from ...config.logging_config import *
+
+
+class Job:
+    def __init__(self, channel, token, crn, provider_job_id, user_identity):
+        self.channel = channel if channel else "ibm_quantum"
+        self.token = token if token else ""
+        self.crn = crn
+        self.job_id = provider_job_id if provider_job_id else ""
+        self.retrieve_job = self.__get_job()
+        self.user_identity = user_identity
+
+    def fetch_job(self) -> JobResponse:
+        logger.info("Start get job info.")
+
+        provider_job_id = self._get_provider_job_id()
+        job_status = self._get_job_status()
+        job_result_dictionary = {}
+        content_type = None
+        job_histogram = None
+        execution_time = None
+
+        try:
+            if JobStatus.DONE.value.__eq__(job_status):
+                logger.info("Try to get job result")
+
+                job_result = self.retrieve_job.result()
+                job_status = self._get_job_status()
+
+                logger.info("Parsing job result")
+                job_result_dictionary = self._parse_job_result(job_result)
+
+                content_type = MediaType.APPLICATION_JSON.value
+
+                logger.info("Producing histogram")
+                job_histogram = self._produce_histogram_data(job_result)
+
+                logger.debug('Calculating execution time ....')
+                execution_time = self._get_execution_time(job_result_dictionary)
+                logger.debug('Execution time calculation completed!')
+
+        except Exception as exception:
+
+            logger.info("Try to job result error.")
+            job_result_dictionary = {
+                "error": "Exception when invoke job on device: " + self.retrieve_job.backend().backend_name,
+                "exception": str(exception)
+            }
+
+            job_status = JobStatus.ERROR.value
+
+        return JobResponse(
+            provider_job_id=provider_job_id,
+            job_status=job_status,
+            job_result=job_result_dictionary,
+            content_type=content_type,
+            job_histogram=job_histogram,
+            user_identity=self.user_identity,
+            execution_time=execution_time
+        )
+
+    def __get_job(self):
+        logger.info("Has IBM token: {0}".format((self.token is not None) and (len(self.token) > 0)))
+
+        service = QiskitRuntimeService(channel=self.channel,
+                                       token=self.token,
+                                       instance=self.crn)
+
+        return service.job(job_id=self.job_id)
+
+    def _get_provider_job_id(self) -> str:
+        return self.retrieve_job.job_id()
+
+    def _get_job_status(self) -> str:
+        return self.retrieve_job.status().name
+
+    @staticmethod
+    def _produce_histogram_data(job_result) -> dict:
+        try:
+            histogram_data = job_result.get_counts()
+        except Exception:
+            histogram_data = None
+
+        return histogram_data
+
+    def _parse_job_result(self, job_result):
+        if self.retrieve_job.program_id == 'sampler':
+            return JsonParserUtils.parse(job_result.__dict__)
+        return JsonParserUtils.parse(job_result.to_dict())
+
+    @staticmethod
+    def _get_execution_time(job_result):
+        if 'metadata' not in job_result:
+            return None
+
+        metadata = job_result['metadata']
+
+        if metadata is None \
+                or not bool(metadata) \
+                or 'time_taken_execute' not in metadata:
+            return None
+
+        return metadata['time_taken_execute']
```

### Comparing `quao-0.3.6/src/quao/model/provider/aws_braket_provider.py` & `quao-0.3.7/src/quao/model/provider/aws_braket_provider.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    QuaO Project aws_braket_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-import boto3
-from braket.aws import AwsSession, AwsDevice
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import *
-
-
-class AwsBraketProvider(Provider):
-
-    def __init__(self, aws_access_key, aws_secret_access_key, region_name):
-        super().__init__(ProviderType.AWS_BRAKET)
-        self.aws_access_key = aws_access_key
-        self.aws_secret_access_key = aws_secret_access_key
-        self.region_name = region_name
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        """
-
-        session = self.collect_providers()
-        return AwsDevice(
-            arn=device_specification,
-            aws_session=session)
-
-    def collect_providers(self):
-        """
-
-        """
-
-        logger.debug('Connect to Aws Braket provider')
-        session = boto3.Session(
-            aws_access_key_id=self.aws_access_key,
-            aws_secret_access_key=self.aws_secret_access_key,
-            region_name=self.region_name)
-
-        return AwsSession(boto_session=session)
+"""
+    QuaO Project aws_braket_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+import boto3
+from braket.aws import AwsSession, AwsDevice
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from ...config.logging_config import *
+
+
+class AwsBraketProvider(Provider):
+
+    def __init__(self, aws_access_key, aws_secret_access_key, region_name):
+        super().__init__(ProviderType.AWS_BRAKET)
+        self.aws_access_key = aws_access_key
+        self.aws_secret_access_key = aws_secret_access_key
+        self.region_name = region_name
+
+    def get_backend(self, device_specification: str):
+        """
+
+        @param device_specification:
+        """
+
+        session = self.collect_providers()
+        return AwsDevice(
+            arn=device_specification,
+            aws_session=session)
+
+    def collect_providers(self):
+        """
+
+        """
+
+        logger.debug('Connect to Aws Braket provider')
+        session = boto3.Session(
+            aws_access_key_id=self.aws_access_key,
+            aws_secret_access_key=self.aws_secret_access_key,
+            region_name=self.region_name)
+
+        return AwsSession(boto_session=session)
```

### Comparing `quao-0.3.6/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.3.7/src/quao/model/provider/ibm_cloud_provider.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-    QuaO Project ibm_cloud_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_ibm_runtime import QiskitRuntimeService
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import *
-
-
-class IbmCloudProvider(Provider):
-
-    def __init__(self, api_key, crn):
-        super().__init__(ProviderType.IBM_CLOUD)
-        self.api_key = api_key
-        self.crn = crn
-        self.channel = 'ibm_cloud'
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        @return:
-        """
-        provider = self.collect_providers()
-
-        return provider.get_backend(name=device_specification)
-
-    def collect_providers(self):
-        """
-
-        @return:
-        """
-
-        logger.debug('Connect to Ibm Cloud provider')
-        return QiskitRuntimeService(channel=self.channel, token=self.api_key, instance=self.crn)
+"""
+    QuaO Project ibm_cloud_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from qiskit_ibm_runtime import QiskitRuntimeService
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from ...config.logging_config import *
+
+
+class IbmCloudProvider(Provider):
+
+    def __init__(self, api_key, crn):
+        super().__init__(ProviderType.IBM_CLOUD)
+        self.api_key = api_key
+        self.crn = crn
+        self.channel = 'ibm_cloud'
+
+    def get_backend(self, device_specification: str):
+        """
+
+        @param device_specification:
+        @return:
+        """
+        provider = self.collect_providers()
+
+        return provider.get_backend(name=device_specification)
+
+    def collect_providers(self):
+        """
+
+        @return:
+        """
+
+        logger.debug('Connect to Ibm Cloud provider')
+        return QiskitRuntimeService(channel=self.channel, token=self.api_key, instance=self.crn)
```

### Comparing `quao-0.3.6/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.3.7/src/quao/model/provider/provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-"""
-    QuaO Project ibm_quantum_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_ibm_provider import IBMProvider
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from ...config.logging_config import *
-
-
-class IbmQuantumProvider(Provider):
-    def __init__(self, api_token):
-        super().__init__(ProviderType.IBM_QUANTUM)
-        self.api_token = api_token
-
-    def get_backend(self, device_specification: str):
-        """
-
-        @param device_specification:
-        """
-
-        provider = self.collect_providers()
-
-        return provider.get_backend(device_specification)
-
-    def collect_providers(self):
-        """
-
-        @return:
-        """
-
-        logger.debug('Connect to Ibm Quantum provider')
-        return IBMProvider(token=self.api_token)
+"""
+    QuaO Project provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from abc import abstractmethod, ABC
+
+from ...enum.provider_type import ProviderType
+
+
+class Provider(ABC):
+
+    def __init__(self, provider_type: ProviderType):
+        self.provider_type = provider_type
+
+    @abstractmethod
+    def get_backend(self, device_specification):
+        """
+
+        """
+        pass
+
+    @abstractmethod
+    def collect_providers(self):
+        """
+
+        """
+        pass
+
+    def get_provider_type(self):
+        return self.provider_type
```

### Comparing `quao-0.3.6/src/quao/model/provider/quao_provider.py` & `quao-0.3.7/src/quao/model/provider/quao_provider.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""
-    QuaO Project quao_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
-"""
-from qiskit_aer import Aer
-
-from ...enum.provider_type import ProviderType
-from ...model.provider.provider import Provider
-from braket.devices import LocalSimulator
-from ...config.logging_config import *
-
-
-class QuaoProvider(Provider):
-    def __init__(self):
-        super().__init__(ProviderType.QUAO_QUANTUM_SIMULATOR)
-
-    def get_backend(self, device_specification):
-        """
-
-        @param device_specification:
-        @return:
-        """
-
-        providers = self.collect_providers()
-
-        aer_device_names = set(map(self.__map_aer_backend_name, providers[0].backends()))
-        aws_device_names = providers[1].registered_backends()
-
-        if aer_device_names.__contains__(device_specification):
-            backend = providers[0].get_backend(device_specification)
-
-            return backend
-
-        if aws_device_names.__contains__(device_specification):
-            return LocalSimulator(device_specification)
-
-        raise Exception('Unsupported device')
-
-    def collect_providers(self):
-        """
-
-        @return:
-        """
-        logger.debug('Connect to Quao provider')
-        return [Aer, LocalSimulator()]
-
-    @staticmethod
-    def __map_aer_backend_name(backend):
-        return backend.configuration().backend_name
+"""
+    QuaO Project quao_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from qiskit_aer import Aer
+
+from ...enum.provider_type import ProviderType
+from ...model.provider.provider import Provider
+from braket.devices import LocalSimulator
+from ...config.logging_config import *
+
+
+class QuaoProvider(Provider):
+    def __init__(self):
+        super().__init__(ProviderType.QUAO_QUANTUM_SIMULATOR)
+
+    def get_backend(self, device_specification):
+        """
+
+        @param device_specification:
+        @return:
+        """
+
+        providers = self.collect_providers()
+
+        aer_device_names = set(map(self.__map_aer_backend_name, providers[0].backends()))
+        aws_device_names = providers[1].registered_backends()
+
+        if aer_device_names.__contains__(device_specification):
+            backend = providers[0].get_backend(device_specification)
+
+            return backend
+
+        if aws_device_names.__contains__(device_specification):
+            return LocalSimulator(device_specification)
+
+        raise Exception('Unsupported device')
+
+    def collect_providers(self):
+        """
+
+        @return:
+        """
+        logger.debug('Connect to Quao provider')
+        return [Aer, LocalSimulator()]
+
+    @staticmethod
+    def __map_aer_backend_name(backend):
+        return backend.configuration().backend_name
```

### Comparing `quao-0.3.6/src/quao.egg-info/PKG-INFO` & `quao-0.3.7/src/quao.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: quao
-Version: 0.3.6
-Summary: Quao Library supporting Quao Platform for Quantum Computing
-Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
-License: The MIT License (MIT)
-        Copyright © CITYNOW Co. Ltd. All rights reserved.
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://citynow.vn/
-Keywords: quao,quantum
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# quao 
-
-quao is a supporting library for Quantum Computing.
-
-
-
-## Installation
-
-Install quao with pip (Python >=3.10)
-
-```bash
-  pip install quao
-```
-    
-## Usage/Examples
-
-```javascript
-from quao import Backend, RequestData, Utils
-
-# Define sdk name
-sdk = "qiskit"
-
-# Pre-processing input data
-def pre_process(input):
-    data = RequestData(input, sdk)
-    return data
-
-# Post-processing output data
-def post_process(job):
-    output = Utils.counts_post_process(job)
-    return output
-
-
-def handle(event, context):
-    # 1. Pre-processing
-    requestData = pre_process(event)
-
-    # 2. Generate Quantum Circuit
-    qc = generate_circuit(requestData.input)
-
-    # 3. Verify and get Backend information
-    backend = Backend(requestData, qc)
-
-    # 4. Submit job and wait up to 1 min for job to complete.
-    job = backend.submit_job(qc)
-
-    # 5. Post-process
-    if job.jobResult:
-        job = post_process(job)
-    response = Utils.generate_response(job)
-
-    # 6. Send back the result
-    return response
-```
-
-
-## Authors
-
-- [CITYNOW Co. Ltd.](https://citynow.vn/)
-
-
-## Documentation
-
-TBA
-
+Metadata-Version: 2.1
+Name: quao
+Version: 0.3.7
+Summary: Quao Library supporting Quao Platform for Quantum Computing
+Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
+License: The MIT License (MIT)
+        Copyright © CITYNOW Co. Ltd. All rights reserved.
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://citynow.vn/
+Keywords: quao,quantum
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# quao 
+
+quao is a supporting library for Quantum Computing.
+
+
+
+## Installation
+
+Install quao with pip (Python >=3.10)
+
+```bash
+  pip install quao
+```
+    
+## Usage/Examples
+
+```javascript
+from quao import Backend, RequestData, Utils
+
+# Define sdk name
+sdk = "qiskit"
+
+# Pre-processing input data
+def pre_process(input):
+    data = RequestData(input, sdk)
+    return data
+
+# Post-processing output data
+def post_process(job):
+    output = Utils.counts_post_process(job)
+    return output
+
+
+def handle(event, context):
+    # 1. Pre-processing
+    requestData = pre_process(event)
+
+    # 2. Generate Quantum Circuit
+    qc = generate_circuit(requestData.input)
+
+    # 3. Verify and get Backend information
+    backend = Backend(requestData, qc)
+
+    # 4. Submit job and wait up to 1 min for job to complete.
+    job = backend.submit_job(qc)
+
+    # 5. Post-process
+    if job.jobResult:
+        job = post_process(job)
+    response = Utils.generate_response(job)
+
+    # 6. Send back the result
+    return response
+```
+
+
+## Authors
+
+- [CITYNOW Co. Ltd.](https://citynow.vn/)
+
+
+## Documentation
+
+TBA
+
```

### Comparing `quao-0.3.6/src/quao.egg-info/SOURCES.txt` & `quao-0.3.7/src/quao.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 src/__init__.py
 src/quao/__init__.py
 src/quao/backend.py
+src/quao/invocation_handler.py
 src/quao.egg-info/PKG-INFO
 src/quao.egg-info/SOURCES.txt
 src/quao.egg-info/dependency_links.txt
 src/quao.egg-info/requires.txt
 src/quao.egg-info/top_level.txt
 src/quao/config/__init__.py
 src/quao/config/logging_config.py
```

