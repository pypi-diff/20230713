# Comparing `tmp/alibabacloud_cms20190101-2.0.6.tar.gz` & `tmp/alibabacloud_cms20190101-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.6.tar", last modified: Thu May 11 08:00:43 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cms20190101-2.0.7.tar", last modified: Thu Jul 13 10:49:10 2023, max compression
```

## Comparing `alibabacloud_cms20190101-2.0.6.tar` & `alibabacloud_cms20190101-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2338 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   664733 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/client.py
--rw-r--r--   0 root         (0) root         (0)  1801777 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2338 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2620 2023-05-11 08:00:43.000000 alibabacloud_cms20190101-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   666677 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1807690 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-07-13 10:49:10.000000 alibabacloud_cms20190101-2.0.7/setup.py
```

### Comparing `alibabacloud_cms20190101-2.0.6/LICENSE` & `alibabacloud_cms20190101-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.6/PKG-INFO` & `alibabacloud_cms20190101-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cms20190101
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.6/README-CN.md` & `alibabacloud_cms20190101-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.6/README.md` & `alibabacloud_cms20190101-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/client.py` & `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4902,14 +4902,15 @@
     def describe_alert_history_list_with_options(
         self,
         request: cms_20190101_models.DescribeAlertHistoryListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeAlertHistoryListResponse:
         """
         @deprecated : DescribeAlertHistoryList is deprecated, please use Cms::2019-01-01::DescribeAlertLogList instead.
+        This API operation is no longer maintained. We recommend that you call the [DescribeAlertLogList](~~201087~~) operation.
         
         @param request: DescribeAlertHistoryListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeAlertHistoryListResponse
         Deprecated
         """
         UtilClient.validate_model(request)
@@ -4960,14 +4961,15 @@
     async def describe_alert_history_list_with_options_async(
         self,
         request: cms_20190101_models.DescribeAlertHistoryListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeAlertHistoryListResponse:
         """
         @deprecated : DescribeAlertHistoryList is deprecated, please use Cms::2019-01-01::DescribeAlertLogList instead.
+        This API operation is no longer maintained. We recommend that you call the [DescribeAlertLogList](~~201087~~) operation.
         
         @param request: DescribeAlertHistoryListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeAlertHistoryListResponse
         Deprecated
         """
         UtilClient.validate_model(request)
@@ -5017,28 +5019,30 @@
 
     def describe_alert_history_list(
         self,
         request: cms_20190101_models.DescribeAlertHistoryListRequest,
     ) -> cms_20190101_models.DescribeAlertHistoryListResponse:
         """
         @deprecated : DescribeAlertHistoryList is deprecated, please use Cms::2019-01-01::DescribeAlertLogList instead.
+        This API operation is no longer maintained. We recommend that you call the [DescribeAlertLogList](~~201087~~) operation.
         
         @param request: DescribeAlertHistoryListRequest
         @return: DescribeAlertHistoryListResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_alert_history_list_with_options(request, runtime)
 
     async def describe_alert_history_list_async(
         self,
         request: cms_20190101_models.DescribeAlertHistoryListRequest,
     ) -> cms_20190101_models.DescribeAlertHistoryListResponse:
         """
         @deprecated : DescribeAlertHistoryList is deprecated, please use Cms::2019-01-01::DescribeAlertLogList instead.
+        This API operation is no longer maintained. We recommend that you call the [DescribeAlertLogList](~~201087~~) operation.
         
         @param request: DescribeAlertHistoryListRequest
         @return: DescribeAlertHistoryListResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_alert_history_list_with_options_async(request, runtime)
@@ -8192,22 +8196,30 @@
     ) -> cms_20190101_models.DescribeMetricRuleBlackListResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.ids):
             query['Ids'] = request.ids
+        if not UtilClient.is_unset(request.instance_ids):
+            query['InstanceIds'] = request.instance_ids
+        if not UtilClient.is_unset(request.is_enable):
+            query['IsEnable'] = request.is_enable
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeMetricRuleBlackList',
             version='2019-01-01',
             protocol='HTTPS',
@@ -8230,22 +8242,30 @@
     ) -> cms_20190101_models.DescribeMetricRuleBlackListResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.ids):
             query['Ids'] = request.ids
+        if not UtilClient.is_unset(request.instance_ids):
+            query['InstanceIds'] = request.instance_ids
+        if not UtilClient.is_unset(request.is_enable):
+            query['IsEnable'] = request.is_enable
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeMetricRuleBlackList',
             version='2019-01-01',
             protocol='HTTPS',
@@ -10221,15 +10241,15 @@
 
     def describe_project_meta_with_options(
         self,
         request: cms_20190101_models.DescribeProjectMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeProjectMetaResponse:
         """
-        The description of the cloud service.
+        The information obtained by this operation includes the service description, namespace, and tags.
         
         @param request: DescribeProjectMetaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeProjectMetaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10260,15 +10280,15 @@
 
     async def describe_project_meta_with_options_async(
         self,
         request: cms_20190101_models.DescribeProjectMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeProjectMetaResponse:
         """
-        The description of the cloud service.
+        The information obtained by this operation includes the service description, namespace, and tags.
         
         @param request: DescribeProjectMetaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeProjectMetaResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10298,28 +10318,28 @@
         )
 
     def describe_project_meta(
         self,
         request: cms_20190101_models.DescribeProjectMetaRequest,
     ) -> cms_20190101_models.DescribeProjectMetaResponse:
         """
-        The description of the cloud service.
+        The information obtained by this operation includes the service description, namespace, and tags.
         
         @param request: DescribeProjectMetaRequest
         @return: DescribeProjectMetaResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_project_meta_with_options(request, runtime)
 
     async def describe_project_meta_async(
         self,
         request: cms_20190101_models.DescribeProjectMetaRequest,
     ) -> cms_20190101_models.DescribeProjectMetaResponse:
         """
-        The description of the cloud service.
+        The information obtained by this operation includes the service description, namespace, and tags.
         
         @param request: DescribeProjectMetaRequest
         @return: DescribeProjectMetaResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_project_meta_with_options_async(request, runtime)
 
@@ -10523,15 +10543,15 @@
 
     def describe_site_monitor_ispcity_list_with_options(
         self,
         request: cms_20190101_models.DescribeSiteMonitorISPCityListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeSiteMonitorISPCityListResponse:
         """
-        The code of the province.
+        This topic provides an example on how to query the detection points that are provided by China Unicom in Guiyang.
         
         @param request: DescribeSiteMonitorISPCityListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSiteMonitorISPCityListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10566,15 +10586,15 @@
 
     async def describe_site_monitor_ispcity_list_with_options_async(
         self,
         request: cms_20190101_models.DescribeSiteMonitorISPCityListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cms_20190101_models.DescribeSiteMonitorISPCityListResponse:
         """
-        The code of the province.
+        This topic provides an example on how to query the detection points that are provided by China Unicom in Guiyang.
         
         @param request: DescribeSiteMonitorISPCityListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSiteMonitorISPCityListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10608,28 +10628,28 @@
         )
 
     def describe_site_monitor_ispcity_list(
         self,
         request: cms_20190101_models.DescribeSiteMonitorISPCityListRequest,
     ) -> cms_20190101_models.DescribeSiteMonitorISPCityListResponse:
         """
-        The code of the province.
+        This topic provides an example on how to query the detection points that are provided by China Unicom in Guiyang.
         
         @param request: DescribeSiteMonitorISPCityListRequest
         @return: DescribeSiteMonitorISPCityListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_site_monitor_ispcity_list_with_options(request, runtime)
 
     async def describe_site_monitor_ispcity_list_async(
         self,
         request: cms_20190101_models.DescribeSiteMonitorISPCityListRequest,
     ) -> cms_20190101_models.DescribeSiteMonitorISPCityListResponse:
         """
-        The code of the province.
+        This topic provides an example on how to query the detection points that are provided by China Unicom in Guiyang.
         
         @param request: DescribeSiteMonitorISPCityListRequest
         @return: DescribeSiteMonitorISPCityListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_site_monitor_ispcity_list_with_options_async(request, runtime)
```

### Comparing `alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101/models.py` & `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12967,26 +12967,66 @@
         region_id: str = None,
         rule_id: str = None,
         rule_name: str = None,
         start_time: str = None,
         state: str = None,
         status: str = None,
     ):
+        # The order of alerts. Valid values:
+        # 
+        # *   true (default value): reverse chronological order
+        # *   false: chronological order
         self.ascending = ascending
+        # The end timestamp of the historical alerts that you want to query.
+        # 
+        # Unit: milliseconds.
         self.end_time = end_time
+        # The ID of the application group.
+        # 
+        # For information about how to obtain the ID of an application group, see [DescribeMonitorGroups](~~115032~~).
         self.group_id = group_id
+        # The metric that is used to monitor the cloud service.
+        # 
+        # For information about how to query the name of a metric, see [Appendix 1: Metrics](~~163515~~).
         self.metric_name = metric_name
+        # The namespace of the cloud service.
+        # 
+        # For information about how to query the namespace of a cloud service, see [Appendix 1: Metrics](~~163515~~).
         self.namespace = namespace
+        # The number of the page to return.
+        # 
+        # Default value: 1.
         self.page = page
+        # The number of entries to return on each page.
+        # 
+        # Default value: 10.
         self.page_size = page_size
         self.region_id = region_id
+        # The ID of the alert rule.
+        # 
+        # For information about how to obtain the ID of an alert rule, see [DescribeMetricRuleList](~~114941~~).
         self.rule_id = rule_id
+        # The name of the alert rule.
+        # 
+        # For information about how to query the name of an alert rule, see [DescribeMetricRuleList](~~114941~~).
         self.rule_name = rule_name
+        # The start timestamp of the historical alerts that you want to query.
+        # 
+        # Unit: milliseconds.
         self.start_time = start_time
+        # The status of the alert. Valid values:
+        # 
+        # *   ALARM (default value): Alerts are triggered.
+        # *   OK: No alerts are triggered.
         self.state = state
+        # Specifies whether alerts are muted. Valid values:
+        # 
+        # *   2 (default value): Alerts are muted and are not triggered within the mute period, even if the condition specified in the alert rule is met.
+        # *   0: Alerts are triggered or cleared.
+        # *   1: The alert rule is ineffective.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13209,34 +13249,69 @@
         rule_id: str = None,
         rule_name: str = None,
         state: str = None,
         status: int = None,
         value: str = None,
         webhooks: str = None,
     ):
+        # The timestamp when the alert was triggered. Unit: milliseconds.
         self.alert_time = alert_time
+        # The TradeManager IDs of the alert contacts.
+        # 
+        # > This parameter is valid only on the China site (aliyun.com).
         self.contact_aliims = contact_aliims
+        # The alert contact groups.
         self.contact_groups = contact_groups
+        # The email addresses of the alert contacts.
         self.contact_mails = contact_mails
+        # The mobile numbers of the alert contacts.
+        # 
+        # > This parameter is valid only on the China site (aliyun.com).
         self.contact_smses = contact_smses
+        # The alert contacts that receive alert notifications.
         self.contacts = contacts
+        # The resources that are monitored.
         self.dimensions = dimensions
+        # The consecutive number of times for which the metric value meets the alert condition before an alert is triggered.
         self.evaluation_count = evaluation_count
+        # The expression that is used to trigger alerts.
         self.expression = expression
+        # The ID of the application group.
         self.group_id = group_id
+        # The instance name.
         self.instance_name = instance_name
+        # The duration of the alert. Unit: milliseconds.
         self.last_time = last_time
+        # The severity level and notification methods of the alert. Valid values:
+        # 
+        # *   P4: Alert notifications are sent by using emails and DingTalk chatbots.
+        # *   OK: No alert is generated.
         self.level = level
+        # The metric name.
         self.metric_name = metric_name
+        # The namespace of the cloud service.
         self.namespace = namespace
+        # The ID of the alert rule.
         self.rule_id = rule_id
+        # The name of the alert rule.
         self.rule_name = rule_name
+        # The alert status. Valid values:
+        # 
+        # *   ALARM: Alerts are triggered.
+        # *   OK: No alerts are triggered.
         self.state = state
+        # Indicates whether alerts are muted. Valid values:
+        # 
+        # *   2 (default): Alerts are muted and are not triggered within the mute period, even if the condition specified in the alert rule is met.
+        # *   0: Alerts are triggered or cleared.
+        # *   1: The alert rule is ineffective.
         self.status = status
+        # The threshold of the metric value to trigger or clear an alert.
         self.value = value
+        # The callback URL.
         self.webhooks = webhooks
 
     def validate(self):
         if self.contact_aliims:
             self.contact_aliims.validate()
         if self.contact_groups:
             self.contact_groups.validate()
@@ -13390,19 +13465,30 @@
         alarm_history_list: DescribeAlertHistoryListResponseBodyAlarmHistoryList = None,
         code: str = None,
         message: str = None,
         request_id: str = None,
         success: bool = None,
         total: str = None,
     ):
+        # The details of historical alerts.
         self.alarm_history_list = alarm_history_list
+        # The status code.
+        # 
+        # > The status code 200 indicates that the request was successful.
         self.code = code
+        # The error message.
         self.message = message
+        # The request ID.
         self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   true
+        # *   false
         self.success = success
+        # The total number of entries returned.
         self.total = total
 
     def validate(self):
         if self.alarm_history_list:
             self.alarm_history_list.validate()
 
     def to_map(self):
@@ -25431,78 +25517,102 @@
 
 
 class DescribeMetricRuleBlackListRequest(TeaModel):
     def __init__(
         self,
         category: str = None,
         ids: List[str] = None,
+        instance_ids: List[str] = None,
+        is_enable: bool = None,
+        name: str = None,
         namespace: str = None,
         order: int = None,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
+        scope_type: str = None,
     ):
         # The ID of the blacklist policy.
         self.category = category
         self.ids = ids
+        self.instance_ids = instance_ids
+        self.is_enable = is_enable
+        self.name = name
         # The timestamp when the blacklist policy expired.
         # 
         # Unit: milliseconds.
         self.namespace = namespace
         # The HTTP status code.
         # 
         # >  The status code 200 indicates that the call was successful.
         self.order = order
         # The name of the metric.
         self.page_number = page_number
         # The categories of the Alibaba Cloud service. For example, ApsaraDB for Redis includes the following categories: ApsaraDB for Redis (standard architecture), ApsaraDB for Redis (cluster architecture), and ApsaraDB for Redis (read/write splitting architecture). In this case, the valid values of this parameter for ApsaraDB for Redis include `kvstore_standard`, `kvstore_sharding`, and `kvstore_splitrw`.
         self.page_size = page_size
         self.region_id = region_id
+        self.scope_type = scope_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.category is not None:
             result['Category'] = self.category
         if self.ids is not None:
             result['Ids'] = self.ids
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.is_enable is not None:
+            result['IsEnable'] = self.is_enable
+        if self.name is not None:
+            result['Name'] = self.name
         if self.namespace is not None:
             result['Namespace'] = self.namespace
         if self.order is not None:
             result['Order'] = self.order
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Category') is not None:
             self.category = m.get('Category')
         if m.get('Ids') is not None:
             self.ids = m.get('Ids')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('IsEnable') is not None:
+            self.is_enable = m.get('IsEnable')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         if m.get('Order') is not None:
             self.order = m.get('Order')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
         return self
 
 
 class DescribeMetricRuleBlackListResponseBodyDescribeMetricRuleBlackListMetrics(TeaModel):
     def __init__(
         self,
         metric_name: str = None,
@@ -33441,41 +33551,33 @@
 class DescribeProjectMetaRequest(TeaModel):
     def __init__(
         self,
         labels: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # Indicates whether the call was successful. The value true indicates success. The value false indicates failure.
-        self.labels = labels
         # The tags. Tags are used to filter services.
         # 
-        # Tags are returned in the following format: `[{"name":"Tag key","value":"Tag value"}, {"name":"Tag key","value":"Tag value"}]`. The following tags are commonly used:
-        # 
-        # *   alertUnit: the unit of the metric value in alerts.
-        # 
-        #     If the unit is small, the original metric value may be too large. In this case, you can use the `alertUnit` tag to specify an appropriate unit. This tag is used in CloudMonitor.
-        # 
-        # *   minAlertPeriod: the minimum time interval to report a new alert. The interval is usually set to 1 minute.
-        # 
-        # *   metricCategory: the specification of the service. Example: kvstore_sharding.
+        # You can filter services only by the tag whose `name` is `product`. Example: {"name":"product","value":"ECS"}.
         # 
-        #     An Alibaba Cloud service may have different specifications that are defined in the same namespace. You can use this parameter to distinguish between service specifications.
+        # > We recommend that you do not use the special tags in the CloudMonitor console.
+        self.labels = labels
+        # The page number.
         # 
-        # *   is_alarm: specifies whether an alert rule can be set.
+        # Valid values: 1 to 100.
         # 
-        #     We recommend that you do not use the special tags in the CloudMonitor console.
+        # Default value: 1.
         self.page_number = page_number
-        # The number of entries to return on each page.
+        # The number of entries per page.
         # 
         # Valid values: 1 to 10000.
         # 
         # Default value: 30.
         # 
-        # >  The value of this parameter is not limited. You can view a large number of entries per page.
+        # > The value of this parameter is not limited. You can view a large number of entries per page.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33505,17 +33607,26 @@
 class DescribeProjectMetaResponseBodyResourcesResource(TeaModel):
     def __init__(
         self,
         description: str = None,
         labels: str = None,
         namespace: str = None,
     ):
+        # The description.
         self.description = description
+        # The tags. Tags are used to filter services.
+        # 
+        # Tags are returned in the following format: `[{"name":"Tag key","value":"Tag value"}, {"name":"Tag key","value":"Tag value"}]`. The following tags are commonly used:
+        # 
+        # *   alertUnit: the unit of the metric value in alerts. If the unit is small, the original metric value may be too large. In this case, you can use the `alertUnit` tag to specify an appropriate unit. This tag is used in CloudMonitor.
+        # *   minAlertPeriod: the minimum time interval to report a new alert. The interval is usually set to 1 minute.
+        # *   metricCategory: the service specification. Example: kvstore_sharding. An Alibaba Cloud service may have different specifications that are defined in the same namespace. You can use this parameter to distinguish between service specifications.
+        # *   is_alarm: specifies whether an alert rule can be set. We recommend that you do not use the special tags in the CloudMonitor console.
         self.labels = labels
-        # The ID of the request.
+        # The namespace of the cloud service. Format: `acs_Service name abbreviation`. For more information about namespaces, see [Appendix 1: Metrics](~~163515~~).
         self.namespace = namespace
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33585,39 +33696,31 @@
         page_number: str = None,
         page_size: str = None,
         request_id: str = None,
         resources: DescribeProjectMetaResponseBodyResources = None,
         success: bool = None,
         total: str = None,
     ):
-        # The tags. Tags are used to filter services.
-        # 
-        # You can filter services only by the tag whose `name` is `product`. Example: {"name":"product","value":"ECS"}.
+        # The status code.
         # 
-        # >  We recommend that you do not use the special tags in the CloudMonitor console.
+        # > The status code 200 indicates that the request was successful.
         self.code = code
         # The error message.
         self.message = message
-        # The number of the page to return.
-        # 
-        # Valid values: 1 to 100.
-        # 
-        # Default value: 1.
+        # The page number.
         self.page_number = page_number
-        # The details of the cloud service.
+        # The number of entries per page.
         self.page_size = page_size
-        # The operation that you want to perform. Set the value to **DescribeProjectMeta**.
+        # The request ID.
         self.request_id = request_id
-        # The number of entries returned per page.
+        # The details of the cloud service.
         self.resources = resources
-        # The HTTP status code.
-        # 
-        # >  The status code 200 indicates that the call was successful.
+        # Indicates whether the request was successful. Valid values: true: The request was successful. false: The request failed.
         self.success = success
-        # The page number of the returned page.
+        # The total number of entries returned.
         self.total = total
 
     def validate(self):
         if self.resources:
             self.resources.validate()
 
     def to_map(self):
@@ -34121,14 +34224,15 @@
         self,
         assertions: DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJsonAssertions = None,
         attempts: int = None,
         authentication: int = None,
         cookie: str = None,
         diagnosis_mtr: bool = None,
         diagnosis_ping: bool = None,
+        dns_hijack_whitelist: str = None,
         dns_match_rule: str = None,
         dns_server: str = None,
         dns_type: str = None,
         expect_value: str = None,
         failure_rate: float = None,
         header: str = None,
         http_method: str = None,
@@ -34149,14 +34253,15 @@
     ):
         self.assertions = assertions
         self.attempts = attempts
         self.authentication = authentication
         self.cookie = cookie
         self.diagnosis_mtr = diagnosis_mtr
         self.diagnosis_ping = diagnosis_ping
+        self.dns_hijack_whitelist = dns_hijack_whitelist
         self.dns_match_rule = dns_match_rule
         self.dns_server = dns_server
         self.dns_type = dns_type
         self.expect_value = expect_value
         self.failure_rate = failure_rate
         self.header = header
         self.http_method = http_method
@@ -34193,14 +34298,16 @@
             result['authentication'] = self.authentication
         if self.cookie is not None:
             result['cookie'] = self.cookie
         if self.diagnosis_mtr is not None:
             result['diagnosis_mtr'] = self.diagnosis_mtr
         if self.diagnosis_ping is not None:
             result['diagnosis_ping'] = self.diagnosis_ping
+        if self.dns_hijack_whitelist is not None:
+            result['dns_hijack_whitelist'] = self.dns_hijack_whitelist
         if self.dns_match_rule is not None:
             result['dns_match_rule'] = self.dns_match_rule
         if self.dns_server is not None:
             result['dns_server'] = self.dns_server
         if self.dns_type is not None:
             result['dns_type'] = self.dns_type
         if self.expect_value is not None:
@@ -34252,14 +34359,16 @@
             self.authentication = m.get('authentication')
         if m.get('cookie') is not None:
             self.cookie = m.get('cookie')
         if m.get('diagnosis_mtr') is not None:
             self.diagnosis_mtr = m.get('diagnosis_mtr')
         if m.get('diagnosis_ping') is not None:
             self.diagnosis_ping = m.get('diagnosis_ping')
+        if m.get('dns_hijack_whitelist') is not None:
+            self.dns_hijack_whitelist = m.get('dns_hijack_whitelist')
         if m.get('dns_match_rule') is not None:
             self.dns_match_rule = m.get('dns_match_rule')
         if m.get('dns_server') is not None:
             self.dns_server = m.get('dns_server')
         if m.get('dns_type') is not None:
             self.dns_type = m.get('dns_type')
         if m.get('expect_value') is not None:
@@ -34301,24 +34410,26 @@
         return self
 
 
 class DescribeSiteMonitorAttributeResponseBodySiteMonitors(TeaModel):
     def __init__(
         self,
         address: str = None,
+        agent_group: str = None,
         interval: str = None,
         isp_cities: DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCities = None,
         option_json: DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJson = None,
         task_id: str = None,
         task_name: str = None,
         task_state: str = None,
         task_type: str = None,
     ):
         # The information of detection points. The information includes the carriers that provide the detection points and the cities where the detection points reside.
         self.address = address
+        self.agent_group = agent_group
         # The name of the site monitoring task.
         self.interval = interval
         # The name of the carrier.
         self.isp_cities = isp_cities
         self.option_json = option_json
         # The ID of the city.
         self.task_id = task_id
@@ -34342,14 +34453,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.address is not None:
             result['Address'] = self.address
+        if self.agent_group is not None:
+            result['AgentGroup'] = self.agent_group
         if self.interval is not None:
             result['Interval'] = self.interval
         if self.isp_cities is not None:
             result['IspCities'] = self.isp_cities.to_map()
         if self.option_json is not None:
             result['OptionJson'] = self.option_json.to_map()
         if self.task_id is not None:
@@ -34362,14 +34475,16 @@
             result['TaskType'] = self.task_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
+        if m.get('AgentGroup') is not None:
+            self.agent_group = m.get('AgentGroup')
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
         if m.get('IspCities') is not None:
             temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsIspCities()
             self.isp_cities = temp_model.from_map(m['IspCities'])
         if m.get('OptionJson') is not None:
             temp_model = DescribeSiteMonitorAttributeResponseBodySiteMonitorsOptionJson()
@@ -34737,28 +34852,37 @@
         city: str = None,
         ipv4: bool = None,
         ipv6: bool = None,
         isp: str = None,
         region_id: str = None,
         view_all: bool = None,
     ):
-        # The name of the country.
+        # The name or ID of the city.
         # 
-        # >  This parameter can be returned only on the China site (aliyun.com).
+        # > City names support fuzzy match.
         self.city = city
-        # The name of the area.
+        # Specifies whether to query IPv4 probes. Valid values:
+        # 
+        # *   true (default): IPv4 probes are queried.
+        # *   false: IPv4 probes are not queried.
         self.ipv4 = ipv4
-        # The name of the area.
+        # Specifies whether to query IPv6 probes. Valid values:
         # 
-        # >  This parameter can be returned only on the China site (aliyun.com).
+        # *   true (default): IPv6 probes are queried.
+        # *   false: IPv6 probes are not queried.
         self.ipv6 = ipv6
-        # The name of the province.
+        # The name or ID of the carrier.
+        # 
+        # > Carrier names support fuzzy match.
         self.isp = isp
         self.region_id = region_id
-        # The IP address pool.
+        # Specifies whether to return all detection points. Valid values:
+        # 
+        # *   true (default): returns all detection points.
+        # *   false: returns only available detection points.
         self.view_all = view_all
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34843,38 +34967,35 @@
         isp_name_zh_c_n: str = None,
         region: str = None,
         region_en: str = None,
         region_zh_c_n: str = None,
     ):
         self.area_en = area_en
         self.area_zh_c_n = area_zh_c_n
-        # The code of the province.
+        # The city ID.
         self.city = city
         self.city_name_en = city_name_en
         self.city_name_zh_c_n = city_name_zh_c_n
-        # Specifies whether to query IPv4 probes. Valid values:
+        # The country name.
         # 
-        # *   true (default value): IPv4 probes are queried.
-        # *   false: IPv4 probes are not queried.
+        # > This parameter is valid only on the China site (aliyun.com).
         self.country = country
         self.country_en = country_en
         self.country_zh_c_n = country_zh_c_n
+        # The IP address pool.
         self.ippool = ippool
-        # Specifies whether to return all detection points. Valid values:
-        # 
-        # *   true (default value): returns all detection points.
-        # *   false: returns only available detection points.
+        # The number of IPv4 probes.
         self.ipv4probe_count = ipv4probe_count
-        # The ID of the carrier.
+        # The number of IPv6 probes.
         self.ipv6probe_count = ipv6probe_count
-        # The returned message.
+        # The carrier ID.
         self.isp = isp
         self.isp_name_en = isp_name_en
         self.isp_name_zh_c_n = isp_name_zh_c_n
-        # The code of the country.
+        # The province name.
         self.region = region
         self.region_en = region_en
         self.region_zh_c_n = region_zh_c_n
 
     def validate(self):
         if self.ippool:
             self.ippool.validate()
@@ -35001,28 +35122,28 @@
         self,
         code: str = None,
         isp_city_list: DescribeSiteMonitorISPCityListResponseBodyIspCityList = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # This topic provides an example on how to query the detection points that are provided by China Unicom in Guiyang.
+        # The status code.
+        # 
+        # > The status code 200 indicates that the request was successful.
         self.code = code
-        # The IP address pool.
+        # The queried detection points.
         self.isp_city_list = isp_city_list
-        # Indicates whether the call was successful. Valid values:
-        # 
-        # *   true: The call was successful.
-        # *   false: The call failed.
+        # The returned message.
         self.message = message
-        # The detection points.
+        # The request ID.
         self.request_id = request_id
-        # The HTTP status code.
+        # Indicates whether the request was successful. Valid values:
         # 
-        # >  The status code 200 indicates that the call was successful.
+        # *   true
+        # *   false
         self.success = success
 
     def validate(self):
         if self.isp_city_list:
             self.isp_city_list.validate()
 
     def to_map(self):
@@ -35530,25 +35651,27 @@
         return self
 
 
 class DescribeSiteMonitorListResponseBodySiteMonitorsSiteMonitor(TeaModel):
     def __init__(
         self,
         address: str = None,
+        agent_group: str = None,
         create_time: str = None,
         interval: str = None,
         options_json: DescribeSiteMonitorListResponseBodySiteMonitorsSiteMonitorOptionsJson = None,
         task_id: str = None,
         task_name: str = None,
         task_state: str = None,
         task_type: str = None,
         update_time: str = None,
     ):
         # The site monitoring tasks that are returned.
         self.address = address
+        self.agent_group = agent_group
         # The keyword to be matched.
         # 
         # >  You can search for tasks by name or address. Fuzzy search is supported.
         self.create_time = create_time
         # The protocol type of DNS detection. Valid values:
         # 
         # *   udp (default value)
@@ -35585,14 +35708,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.address is not None:
             result['Address'] = self.address
+        if self.agent_group is not None:
+            result['AgentGroup'] = self.agent_group
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.interval is not None:
             result['Interval'] = self.interval
         if self.options_json is not None:
             result['OptionsJson'] = self.options_json.to_map()
         if self.task_id is not None:
@@ -35607,14 +35732,16 @@
             result['UpdateTime'] = self.update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
+        if m.get('AgentGroup') is not None:
+            self.agent_group = m.get('AgentGroup')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
         if m.get('OptionsJson') is not None:
             temp_model = DescribeSiteMonitorListResponseBodySiteMonitorsSiteMonitorOptionsJson()
             self.options_json = temp_model.from_map(m['OptionsJson'])
```

### Comparing `alibabacloud_cms20190101-2.0.6/alibabacloud_cms20190101.egg-info/PKG-INFO` & `alibabacloud_cms20190101-2.0.7/alibabacloud_cms20190101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cms20190101
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cms20190101-2.0.6/setup.py` & `alibabacloud_cms20190101-2.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cms20190101.
 
-Created on 11/05/2023
+Created on 13/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cms20190101"
 NAME = "alibabacloud_cms20190101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Monitor (20190101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

