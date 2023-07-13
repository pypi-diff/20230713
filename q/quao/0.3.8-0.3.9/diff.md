# Comparing `tmp/quao-0.3.8.tar.gz` & `tmp/quao-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.3.8.tar", last modified: Thu Jul 13 07:44:55 2023, max compression
+gzip compressed data, was "quao-0.3.9.tar", last modified: Thu Jul 13 07:49:43 2023, max compression
```

## Comparing `quao-0.3.8.tar` & `quao-0.3.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.977482 quao-0.3.8/
--rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-07-13 07:44:55.977482 quao-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.8/README.md
--rw-rw-rw-   0        0        0      967 2023-07-13 07:44:21.000000 quao-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 07:44:55.978483 quao-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.922298 quao-0.3.8/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.925299 quao-0.3.8/src/quao/
--rw-rw-rw-   0        0        0      262 2023-07-13 07:44:21.000000 quao-0.3.8/src/quao/__init__.py
--rw-rw-rw-   0        0        0     7544 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.946299 quao-0.3.8/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.8/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.8/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.947301 quao-0.3.8/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.948299 quao-0.3.8/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.8/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.949864 quao-0.3.8/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.8/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.956604 quao-0.3.8/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.8/src/quao/enum/http_header.py
--rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.8/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.8/src/quao/enum/processing_unit.py
--rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/enum/sdk.py
--rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.8/src/quao/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.959635 quao-0.3.8/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.8/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.8/src/quao/factory/provider_factory.py
--rw-rw-rw-   0        0        0      691 2023-07-13 04:03:48.000000 quao-0.3.8/src/quao/invocation_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.960604 quao-0.3.8/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.967603 quao-0.3.8/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     2463 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3612 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.8/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      788 2023-07-12 04:24:43.000000 quao-0.3.8/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0     1170 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     3337 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.968604 quao-0.3.8/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     3938 2023-07-13 04:03:03.000000 quao-0.3.8/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.974238 quao-0.3.8/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.8/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.8/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.8/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.8/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.8/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.976481 quao-0.3.8/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.8/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.8/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.8/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:44:55.944297 quao-0.3.8/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-07-13 07:44:55.000000 quao-0.3.8/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2023-07-13 07:44:55.000000 quao-0.3.8/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 07:44:55.000000 quao-0.3.8/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      201 2023-07-13 07:44:55.000000 quao-0.3.8/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 07:44:55.000000 quao-0.3.8/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.053020 quao-0.3.9/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 04:30:40.000000 quao-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-07-13 07:49:43.053020 quao-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-05-26 04:30:40.000000 quao-0.3.9/README.md
+-rw-rw-rw-   0        0        0      967 2023-07-13 07:49:22.000000 quao-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:49:43.054021 quao-0.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:42.987010 quao-0.3.9/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:42.991011 quao-0.3.9/src/quao/
+-rw-rw-rw-   0        0        0      262 2023-07-13 07:49:22.000000 quao-0.3.9/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     7544 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.016021 quao-0.3.9/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 09:43:03.000000 quao-0.3.9/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.017021 quao-0.3.9/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.018023 quao-0.3.9/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-07-12 01:46:07.000000 quao-0.3.9/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.020021 quao-0.3.9/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.030036 quao-0.3.9/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      185 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/http_header.py
+-rw-rw-rw-   0        0        0      212 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/enum/sdk.py
+-rw-rw-rw-   0        0        0      169 2023-06-22 02:52:41.000000 quao-0.3.9/src/quao/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.032024 quao-0.3.9/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/factory/provider_factory.py
+-rw-rw-rw-   0        0        0      751 2023-07-13 07:49:10.000000 quao-0.3.9/src/quao/invocation_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.033021 quao-0.3.9/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.039021 quao-0.3.9/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     2463 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3612 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1008 2023-07-07 07:51:32.000000 quao-0.3.9/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      788 2023-07-12 04:24:43.000000 quao-0.3.9/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0     1170 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     3337 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.041022 quao-0.3.9/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     3938 2023-07-13 04:03:03.000000 quao-0.3.9/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.048023 quao-0.3.9/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1004 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      874 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1397 2023-06-29 09:59:18.000000 quao-0.3.9/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.052021 quao-0.3.9/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-06-02 01:59:38.000000 quao-0.3.9/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 10:41:04.000000 quao-0.3.9/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1631 2023-07-12 01:46:07.000000 quao-0.3.9/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:49:43.014024 quao-0.3.9/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1568 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      201 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 07:49:42.000000 quao-0.3.9/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.3.8/LICENSE` & `quao-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/PKG-INFO` & `quao-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.8
+Version: 0.3.9
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.8/README.md` & `quao-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/pyproject.toml` & `quao-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.3.8"
+version = "0.3.9"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.3.8/src/quao/backend.py` & `quao-0.3.9/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/data/job/job_response.py` & `quao-0.3.9/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/data/request/request_data.py` & `quao-0.3.9/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/factory/device_factory.py` & `quao-0.3.9/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/factory/provider_factory.py` & `quao-0.3.9/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/aws_braket_device.py` & `quao-0.3.9/src/quao/model/device/aws_braket_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/device.py` & `quao-0.3.9/src/quao/model/device/device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/ibm_cloud_device.py` & `quao-0.3.9/src/quao/model/device/ibm_cloud_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/ibm_quantum_device.py` & `quao-0.3.9/src/quao/model/device/ibm_quantum_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/qiskit_device.py` & `quao-0.3.9/src/quao/model/device/qiskit_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/device/quao_device.py` & `quao-0.3.9/src/quao/model/device/quao_device.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/job/qiskit_status.py` & `quao-0.3.9/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/provider/aws_braket_provider.py` & `quao-0.3.9/src/quao/model/provider/aws_braket_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.3.9/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.3.9/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/provider/provider.py` & `quao-0.3.9/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/model/provider/quao_provider.py` & `quao-0.3.9/src/quao/model/provider/quao_provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/util/json_parser_util.py` & `quao-0.3.9/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao/util/response_utils.py` & `quao-0.3.9/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.3.8/src/quao.egg-info/PKG-INFO` & `quao-0.3.9/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.3.8
+Version: 0.3.9
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.3.8/src/quao.egg-info/SOURCES.txt` & `quao-0.3.9/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

