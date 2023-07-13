# Comparing `tmp/xj_invoice-1.0.7.tar.gz` & `tmp/xj_invoice-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_invoice-1.0.7.tar", last modified: Wed Jun  7 10:45:03 2023, max compression
+gzip compressed data, was "xj_invoice-1.0.9.tar", last modified: Mon Jun 12 08:31:47 2023, max compression
```

## Comparing `xj_invoice-1.0.7.tar` & `xj_invoice-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.830214 xj_invoice-1.0.7/
--rw-rw-rw-   0        0        0     1616 2023-06-07 10:45:03.829194 xj_invoice-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 10:45:03.830214 xj_invoice-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-07 10:42:01.000000 xj_invoice-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.747124 xj_invoice-1.0.7/xj_invoice/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/__init__.py
--rw-rw-rw-   0        0        0     1629 2023-06-06 07:43:16.000000 xj_invoice-1.0.7/xj_invoice/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.776086 xj_invoice-1.0.7/xj_invoice/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/apis/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-06-05 06:05:16.000000 xj_invoice-1.0.7/xj_invoice/apis/invoice_apis.py
--rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.7/xj_invoice/apis/invoice_type_apis.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.7/xj_invoice/apis/router.py
--rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.7/xj_invoice/apps.py
--rw-rw-rw-   0        0        0    18769 2023-06-06 07:39:16.000000 xj_invoice-1.0.7/xj_invoice/models.py
--rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.7/xj_invoice/service_register.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.792371 xj_invoice-1.0.7/xj_invoice/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/services/__init__.py
--rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.7/xj_invoice/services/invoice_extend_service.py
--rw-rw-rw-   0        0        0    15953 2023-06-07 08:44:07.000000 xj_invoice-1.0.7/xj_invoice/services/invoice_service.py
--rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.7/xj_invoice/services/invoice_type_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/tests.py
--rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.7/xj_invoice/urls.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.827687 xj_invoice-1.0.7/xj_invoice/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/utils/__init__.py
--rw-rw-rw-   0        0        0     4277 2023-05-19 05:46:52.000000 xj_invoice-1.0.7/xj_invoice/utils/custom_response.py
--rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:12.000000 xj_invoice-1.0.7/xj_invoice/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.7/xj_invoice/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.7/xj_invoice/utils/j_dict.py
--rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.7/xj_invoice/utils/join_list.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.7/xj_invoice/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.7/xj_invoice/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.7/xj_invoice/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.7/xj_invoice/views.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:45:03.754328 xj_invoice-1.0.7/xj_invoice.egg-info/
--rw-rw-rw-   0        0        0     1616 2023-06-07 10:45:03.000000 xj_invoice-1.0.7/xj_invoice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-06-07 10:45:03.000000 xj_invoice-1.0.7/xj_invoice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:45:03.000000 xj_invoice-1.0.7/xj_invoice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 10:45:03.000000 xj_invoice-1.0.7/xj_invoice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.737510 xj_invoice-1.0.9/
+-rw-rw-rw-   0        0        0     1616 2023-06-12 08:31:47.736530 xj_invoice-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 08:31:47.737510 xj_invoice-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-12 08:31:36.000000 xj_invoice-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.695221 xj_invoice-1.0.9/xj_invoice/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-06-06 07:43:16.000000 xj_invoice-1.0.9/xj_invoice/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.709619 xj_invoice-1.0.9/xj_invoice/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/apis/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-06-05 06:05:16.000000 xj_invoice-1.0.9/xj_invoice/apis/invoice_apis.py
+-rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.9/xj_invoice/apis/invoice_type_apis.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.9/xj_invoice/apis/router.py
+-rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.9/xj_invoice/apps.py
+-rw-rw-rw-   0        0        0    18945 2023-06-12 08:23:36.000000 xj_invoice-1.0.9/xj_invoice/models.py
+-rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.9/xj_invoice/service_register.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.717628 xj_invoice-1.0.9/xj_invoice/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/services/__init__.py
+-rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.9/xj_invoice/services/invoice_extend_service.py
+-rw-rw-rw-   0        0        0    16754 2023-06-12 08:29:38.000000 xj_invoice-1.0.9/xj_invoice/services/invoice_service.py
+-rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.9/xj_invoice/services/invoice_type_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/tests.py
+-rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.9/xj_invoice/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.734505 xj_invoice-1.0.9/xj_invoice/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/utils/__init__.py
+-rw-rw-rw-   0        0        0     4277 2023-05-19 05:46:52.000000 xj_invoice-1.0.9/xj_invoice/utils/custom_response.py
+-rw-rw-rw-   0        0        0    33476 2023-06-07 10:56:49.000000 xj_invoice-1.0.9/xj_invoice/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.9/xj_invoice/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.9/xj_invoice/utils/j_dict.py
+-rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.9/xj_invoice/utils/join_list.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.9/xj_invoice/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.9/xj_invoice/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.9/xj_invoice/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.9/xj_invoice/views.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:31:47.701926 xj_invoice-1.0.9/xj_invoice.egg-info/
+-rw-rw-rw-   0        0        0     1616 2023-06-12 08:31:46.000000 xj_invoice-1.0.9/xj_invoice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-06-12 08:31:46.000000 xj_invoice-1.0.9/xj_invoice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:31:46.000000 xj_invoice-1.0.9/xj_invoice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 08:31:46.000000 xj_invoice-1.0.9/xj_invoice.egg-info/top_level.txt
```

### Comparing `xj_invoice-1.0.7/PKG-INFO` & `xj_invoice-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_invoice
-Version: 1.0.7
+Version: 1.0.9
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.7/README.md` & `xj_invoice-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/setup.py` & `xj_invoice-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_invoice',  # 模块名称
-    version='1.0.7',  # 模块版本
+    version='1.0.9',  # 模块版本
     description='发票模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='高栋天',  # 作者
     author_email='1499593644@qq.com',  # 作者邮箱
     maintainer=["高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_invoice-1.0.7/xj_invoice/admin.py` & `xj_invoice-1.0.9/xj_invoice/admin.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/apis/invoice_apis.py` & `xj_invoice-1.0.9/xj_invoice/apis/invoice_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/apis/invoice_type_apis.py` & `xj_invoice-1.0.9/xj_invoice/apis/invoice_type_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/apis/middleware.py` & `xj_invoice-1.0.9/xj_invoice/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/apis/router.py` & `xj_invoice-1.0.9/xj_invoice/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/models.py` & `xj_invoice-1.0.9/xj_invoice/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     destroy_date = models.DateTimeField(verbose_name='退回作废日期', default=timezone.now, help_text='')
     destroy_reason = models.CharField(verbose_name='退回作废原因', max_length=128, blank=True, null=True, help_text='')
     destroy_operator_id = models.IntegerField(verbose_name='退回操作员', primary_key=False, help_text='')
 
     receive_email = models.EmailField(verbose_name='接收邮箱', unique=True, blank=True, help_text='')
     receive_phone = models.CharField(verbose_name='接收手机号', max_length=128, blank=True, null=True, help_text='')
     invoice_snapshot = models.JSONField(verbose_name='发票快照', blank=True, null=True, help_text='')
+    create_time = models.DateTimeField(verbose_name='创建时间', auto_now_add=True)
+    update_time = models.DateTimeField(verbose_name='修改时间', auto_now_add=True)
 
     class Meta:
         db_table = 'invoice_invoice'
         verbose_name_plural = "01. 发票 - 发票表"
 
     def __str__(self):
         return f"{self.id}"
```

### Comparing `xj_invoice-1.0.7/xj_invoice/service_register.py` & `xj_invoice-1.0.9/xj_invoice/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/services/invoice_extend_service.py` & `xj_invoice-1.0.9/xj_invoice/services/invoice_extend_service.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/services/invoice_service.py` & `xj_invoice-1.0.9/xj_invoice/services/invoice_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import sys
 import time
 import os
+import pytz
 import datetime
 from decimal import Decimal
 
 from django.db.models import Q
 from django.db.models import F
 from django.forms import model_to_dict
-
+from django.utils import timezone
 from utils.custom_tool import filter_result_field
 from xj_invoice.utils.join_list import JoinList
 from xj_thread.services.thread_list_service import ThreadListService
 from xj_user.services.user_service import UserService
 from ..services.invoice_extend_service import InvoiceExtendService
 from ..utils.custom_tool import format_params_handle, force_transform_type, filter_fields_handler, dynamic_load_class, \
     write_to_log
@@ -125,14 +126,15 @@
         main_form_data['invoice_snapshot'] = json.loads(
             json.dumps(invoice_snapshot, default=decimal_default, ensure_ascii=False))
         # IO操作
         try:
             # 主表插入数据
 
             main_form_data['invoice_status'] = "APPLY"
+            # main_form_data['create_time'] = InvoiceService.get_current_time()
             instance = Invoice.objects.create(**main_form_data)
             # 扩展表 插入或更新
             add_extend_res, err = InvoiceExtendService.create_or_update(params, instance.id)
             if err:
                 write_to_log(prefix="发票--扩展表 插入或更新失败", err_obj=err)
 
             # 载入模块
@@ -220,14 +222,15 @@
 
         update_total = invoice_obj.count()
         if update_total == 0:
             return None, "没有找到可修改项目"
 
         # IO 操作
         try:
+            params['update_time'] = InvoiceService.get_current_time()
             invoice_obj.update(**params)
         except Exception as e:
             return None, "修改异常:" + str(e)
         return invoice_obj.first().to_json(), None
 
     @staticmethod
     def list(params):
@@ -368,7 +371,18 @@
                 lst = [int(value)]
         elif isinstance(value, int):
             lst = [value]
         else:
             raise TypeError("Unsupported value type. Expected string or int.")
 
         return lst
+
+    # 获取当前时间
+    @staticmethod
+    def get_current_time():
+        # TODO USE_TZ = False 时会报错 如果USE_TZ设置为True时，Django会使用系统默认设置的时区，即America/Chicago，此时的TIME_ZONE不管有没有设置都不起作用。
+        tz = pytz.timezone('Asia/Shanghai')
+        # 返回datetime格式的时间
+        now_time = timezone.now().astimezone(tz=tz).strftime("%Y-%m-%d %H:%M:%S")
+        # now = datetime.strptime(now_time, '%Y-%m-%d %H:%M:%S')
+        now = datetime.datetime.strptime(now_time, "%Y-%m-%d %H:%M:%S")
+        return now
```

### Comparing `xj_invoice-1.0.7/xj_invoice/urls.py` & `xj_invoice-1.0.9/xj_invoice/urls.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/custom_response.py` & `xj_invoice-1.0.9/xj_invoice/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/custom_tool.py` & `xj_invoice-1.0.9/xj_invoice/utils/custom_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -481,15 +481,15 @@
             data = {}
 
     else:
         data = getattr(request, 'data', {})
     return {k: v for k, v in data.items()}
 
 
-# 请求参数解析
+# 请求参数析解
 def request_params_wrapper(func):
     # 解析请求参数 兼容 APIView与View的情况，View 没有request.data
     def wrapper(instance, arg_request=None, *args, request=None, **kwargs):
         """
         解析request参数，适配多种body格式。
         PS :注意使用该装饰器之后必搭配*args，**kwargs须使用
         @param instance 实例是一个APIView的实例
@@ -591,62 +591,91 @@
 
 
 # 流程调用装饰器
 def flow_service_wrapper(func):
     """
     API 流程中间件装饰器
     PS 该装饰器必须配套request_params_wrapper 和 user_wrapper 一起使用
+    PS 开放的服务必须使用key_value类型接收参数，如：params: dict = None, **kwargs
     """
 
     # 解析请求参数 兼容 APIView与View的情况，View 没有request.data
     def wrapper(instance, arg_request=None, *args, request=None, request_params=None, user_info: dict = None, **kwargs):
         """
         @param instance 实例是一个APIView的实例
         @param args 其它可变参数元组
         @param kwargs 其它可变关键字参数字典
         :param user_info: 用户信息，使用用户登录验证装饰器才会生效。
         :param request_params: 请求参数解析
         """
-        user_info, is_pass = force_transform_type(variable=user_info, var_type="dict", default={})
         if isinstance(instance, WSGIRequest) or isinstance(instance, Request) or isinstance(instance, ASGIRequest):
             request = instance
         if isinstance(arg_request, WSGIRequest) or isinstance(arg_request, Request) or isinstance(arg_request, ASGIRequest):
             request = arg_request
-        if request_params is None:
-            request_params = {}
-        # 加载流程类
-        CopyFlowProcessService, is_import = dynamic_load_class(import_path="xj_flow.services.flow_process_service", class_name="FlowProcessService")
 
+        # ----------------- section 得到请求参数以及用户信息 start --------------------------
+        user_info, is_pass = force_transform_type(variable=user_info, var_type="dict", default={})
+        request_params, is_pass = force_transform_type(variable=request_params, var_type="dict", default={})
+        # 自动补全，用户信息字段
+        for k, v in user_info.items():
+            request_params.setdefault(k, v)
+        # ----------------- section 得到请求参数以及用户信息 end   --------------------------
+
+        # ----------------- section 加载流程类,并判断是否要执行流程 start --------------------------
+        CopyFlowProcessService, is_import = dynamic_load_class(import_path="xj_flow.services.flow_process_service", class_name="FlowProcessService")
         # 检查请求参数中是否由流程相关信息,判断是触发流程
         flow_node_id = request_params.pop("flow_node_id", None)
         flow_action_id = request_params.pop("flow_action_id", None)
         flow_node_value = request_params.pop("flow_node_value", None)
         flow_action_value = request_params.pop("flow_action_value", None)
         if is_import or (not flow_node_id and not flow_node_value) or (not flow_action_id and not flow_action_value):
             return func(instance, *args, request=request, request_params=request_params, user_info=user_info.copy(), **kwargs)
+        # ----------------- section 加载流程类,并判断是否要执行流程 end   --------------------------
 
-        # 执行流程
+        # ----------------- section 执行前置流程方法 start --------------------------
         service = CopyFlowProcessService()
         data, err = service.do_once_flow_in_service(
             flow_node_id=flow_node_id,
             flow_node_value=flow_node_value,
             flow_action_id=flow_action_id,
             flow_action_value=flow_action_value,
-            source_params=request_params.copy()
+            source_params=request_params.copy(),
+            run_mode="BEFORE"
         )
+        # 如果有错误则计入执行错误日志
         if err:
             write_to_log(prefix="流程装饰器调用异常:", content=err)
-
-        # 流程执行接口
+        # 处理后的参数默认值补全
+        data = data or {}
         request_params = data.get("source_params", request_params)
-        response = func(instance, *args, request=request, request_params=request_params.copy(), user_info=user_info.copy(), **kwargs)
+        # ----------------- section 执行前置流程方法 end   --------------------------
 
+        # ----------------- section 执行接口方法 start --------------------------
+        response = func(instance, *args, request=request, request_params=request_params.copy(), user_info=user_info.copy(), **kwargs)
         # 获取http响应的内容
         response_json = parse_json(response.content.decode(encoding="utf-8"))
         response_json, is_pass = force_transform_type(variable=response_json, var_type="dict", default={})
+        response_err = response_json.get("err", None)
+        # ----------------- section 执行接口方法 end   --------------------------
+
+        # ----------------- section 执行后置流程方法 start --------------------------
+        if not response_err:
+            # 如果请求接口没有报错则不可以执行
+            data, err = service.do_once_flow_in_service(
+                flow_node_id=flow_node_id,
+                flow_node_value=flow_node_value,
+                flow_action_id=flow_action_id,
+                flow_action_value=flow_action_value,
+                source_params=request_params.copy(),
+                run_mode="AFTER"
+            )
+            if err:
+                write_to_log(prefix="流程装饰器调用异常:", content=err)
+        # ----------------- section 执行后置流程方法 end   --------------------------
+        # 记录流程记录
         record, record_err = service.save_record(result_dict=response_json.get("data", {}), user_info=user_info.copy())
         if record_err:
             write_to_log(prefix="流程装饰器保存流程记录失败", content=record_err)
         return response
 
     return wrapper
```

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/j_config.py` & `xj_invoice-1.0.9/xj_invoice/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/join_list.py` & `xj_invoice-1.0.9/xj_invoice/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/jt.py` & `xj_invoice-1.0.9/xj_invoice/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/model_handle.py` & `xj_invoice-1.0.9/xj_invoice/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/utils/user_wrapper.py` & `xj_invoice-1.0.9/xj_invoice/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice/views.py` & `xj_invoice-1.0.9/xj_invoice/views.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.7/xj_invoice.egg-info/PKG-INFO` & `xj_invoice-1.0.9/xj_invoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-invoice
-Version: 1.0.7
+Version: 1.0.9
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.7/xj_invoice.egg-info/SOURCES.txt` & `xj_invoice-1.0.9/xj_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

