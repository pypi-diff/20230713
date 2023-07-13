# Comparing `tmp/alibabacloud_btripopen20220520-1.1.7.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.7.tar", last modified: Tue Jul  4 01:58:44 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.8.tar", last modified: Thu Jul 13 05:55:44 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.7.tar` & `alibabacloud_btripopen20220520-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/
--rw-r--r--   0 root         (0) root         (0)     3617 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   525626 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1984800 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-04 01:58:44.000000 alibabacloud_btripopen20220520-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-07-04 01:58:43.000000 alibabacloud_btripopen20220520-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525626 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1985099 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 05:55:44.000000 alibabacloud_btripopen20220520-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-07-13 05:55:43.000000 alibabacloud_btripopen20220520-1.1.8/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.7/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.8/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-04 Version: 1.1.7
+- Update.
+
 2023-06-26 Version: 1.1.6
 - Update.
 
 2023-06-16 Version: 1.1.5
 - Update.
 
 2023-06-15 Version: 1.1.4
```

### Comparing `alibabacloud_btripopen20220520-1.1.7/LICENSE` & `alibabacloud_btripopen20220520-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.7/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.7/README-CN.md` & `alibabacloud_btripopen20220520-1.1.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.7/README.md` & `alibabacloud_btripopen20220520-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -37270,25 +37270,27 @@
 class HotelOrderPreValidateResponseBodyModuleRatePlanInfo(TeaModel):
     def __init__(
         self,
         bed_desc: str = None,
         btrip_hotel_cancel_policy_dto: HotelOrderPreValidateResponseBodyModuleRatePlanInfoBtripHotelCancelPolicyDTO = None,
         earliest_check_in_time: str = None,
         latest_check_out_time: str = None,
+        max_booking_num: int = None,
         max_occupancy_num: int = None,
         need_certificate: bool = None,
         need_email: bool = None,
         need_english_name: bool = None,
         total_order_price: int = None,
         total_room_price: int = None,
     ):
         self.bed_desc = bed_desc
         self.btrip_hotel_cancel_policy_dto = btrip_hotel_cancel_policy_dto
         self.earliest_check_in_time = earliest_check_in_time
         self.latest_check_out_time = latest_check_out_time
+        self.max_booking_num = max_booking_num
         self.max_occupancy_num = max_occupancy_num
         self.need_certificate = need_certificate
         self.need_email = need_email
         self.need_english_name = need_english_name
         self.total_order_price = total_order_price
         self.total_room_price = total_room_price
 
@@ -37306,14 +37308,16 @@
             result['bed_desc'] = self.bed_desc
         if self.btrip_hotel_cancel_policy_dto is not None:
             result['btrip_hotel_cancel_policy_d_t_o'] = self.btrip_hotel_cancel_policy_dto.to_map()
         if self.earliest_check_in_time is not None:
             result['earliest_check_in_time'] = self.earliest_check_in_time
         if self.latest_check_out_time is not None:
             result['latest_check_out_time'] = self.latest_check_out_time
+        if self.max_booking_num is not None:
+            result['max_booking_num'] = self.max_booking_num
         if self.max_occupancy_num is not None:
             result['max_occupancy_num'] = self.max_occupancy_num
         if self.need_certificate is not None:
             result['need_certificate'] = self.need_certificate
         if self.need_email is not None:
             result['need_email'] = self.need_email
         if self.need_english_name is not None:
@@ -37331,14 +37335,16 @@
         if m.get('btrip_hotel_cancel_policy_d_t_o') is not None:
             temp_model = HotelOrderPreValidateResponseBodyModuleRatePlanInfoBtripHotelCancelPolicyDTO()
             self.btrip_hotel_cancel_policy_dto = temp_model.from_map(m['btrip_hotel_cancel_policy_d_t_o'])
         if m.get('earliest_check_in_time') is not None:
             self.earliest_check_in_time = m.get('earliest_check_in_time')
         if m.get('latest_check_out_time') is not None:
             self.latest_check_out_time = m.get('latest_check_out_time')
+        if m.get('max_booking_num') is not None:
+            self.max_booking_num = m.get('max_booking_num')
         if m.get('max_occupancy_num') is not None:
             self.max_occupancy_num = m.get('max_occupancy_num')
         if m.get('need_certificate') is not None:
             self.need_certificate = m.get('need_certificate')
         if m.get('need_email') is not None:
             self.need_email = m.get('need_email')
         if m.get('need_english_name') is not None:
```

### Comparing `alibabacloud_btripopen20220520-1.1.7/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.8/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.7
+Version: 1.1.8
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.7/setup.py` & `alibabacloud_btripopen20220520-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 04/07/2023
+Created on 13/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
```

