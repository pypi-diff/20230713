# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.933.tar", last modified: Wed Jul 12 00:21:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.934.tar", last modified: Thu Jul 13 00:17:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.933.tar` & `tencentcloud-sdk-python-cdb-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   151510 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19147 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   831863 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:21:39.000000 tencentcloud-sdk-python-cdb-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   151510 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19147 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   834924 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/setup.py` & `tencentcloud-sdk-python-cdb-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.933'
+__version__ = '3.0.934'
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,22 +809,25 @@
         :type InstanceId: str
         :param _StartTime: 要分析的日志开始时间，格式为："2023-02-16 00:00:20"。
         :type StartTime: str
         :param _EndTime: 要分析的日志结束时间，格式为："2023-02-16 00:10:20"。
         :type EndTime: str
         :param _AggregationConditions: 聚合维度的排序条件。
         :type AggregationConditions: list of AggregationCondition
-        :param _AuditLogFilter: 该过滤条件下的审计日志结果集作为分析日志。
+        :param _AuditLogFilter: 已废弃。该过滤条件下的审计日志结果集作为分析日志。
         :type AuditLogFilter: :class:`tencentcloud.cdb.v20170320.models.AuditLogFilter`
+        :param _LogFilter: 该过滤条件下的审计日志结果集作为分析日志。
+        :type LogFilter: list of InstanceAuditLogFilters
         """
         self._InstanceId = None
         self._StartTime = None
         self._EndTime = None
         self._AggregationConditions = None
         self._AuditLogFilter = None
+        self._LogFilter = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -858,28 +861,42 @@
     def AuditLogFilter(self):
         return self._AuditLogFilter
 
     @AuditLogFilter.setter
     def AuditLogFilter(self, AuditLogFilter):
         self._AuditLogFilter = AuditLogFilter
 
+    @property
+    def LogFilter(self):
+        return self._LogFilter
+
+    @LogFilter.setter
+    def LogFilter(self, LogFilter):
+        self._LogFilter = LogFilter
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         if params.get("AggregationConditions") is not None:
             self._AggregationConditions = []
             for item in params.get("AggregationConditions"):
                 obj = AggregationCondition()
                 obj._deserialize(item)
                 self._AggregationConditions.append(obj)
         if params.get("AuditLogFilter") is not None:
             self._AuditLogFilter = AuditLogFilter()
             self._AuditLogFilter._deserialize(params.get("AuditLogFilter"))
+        if params.get("LogFilter") is not None:
+            self._LogFilter = []
+            for item in params.get("LogFilter"):
+                obj = InstanceAuditLogFilters()
+                obj._deserialize(item)
+                self._LogFilter.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4170,36 +4187,39 @@
 class CreateAuditLogFileRequest(AbstractModel):
     """CreateAuditLogFile请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _InstanceId: 实例 ID，格式如：cdb-c1nl9rpv 或者 cdbro-c1nl9rpv，与云数据库控制台页面中显示的实例 ID 相同。
+        :param _InstanceId: 实例 ID，与云数据库控制台页面中显示的实例 ID 相同。
         :type InstanceId: str
-        :param _StartTime: 开始时间，格式为："2017-07-12 10:29:20"。
+        :param _StartTime: 开始时间。
         :type StartTime: str
-        :param _EndTime: 结束时间，格式为："2017-07-12 10:29:20"。
+        :param _EndTime: 结束时间。
         :type EndTime: str
         :param _Order: 排序方式。支持值包括："ASC" - 升序，"DESC" - 降序。
         :type Order: str
         :param _OrderBy: 排序字段。支持值包括：
 "timestamp" - 时间戳；
 "affectRows" - 影响行数；
 "execTime" - 执行时间。
         :type OrderBy: str
-        :param _Filter: 过滤条件。可按设置的过滤条件过滤日志。
+        :param _Filter: 已废弃。
         :type Filter: :class:`tencentcloud.cdb.v20170320.models.AuditLogFilter`
+        :param _LogFilter: 过滤条件。可按设置的过滤条件过滤日志。
+        :type LogFilter: list of InstanceAuditLogFilters
         """
         self._InstanceId = None
         self._StartTime = None
         self._EndTime = None
         self._Order = None
         self._OrderBy = None
         self._Filter = None
+        self._LogFilter = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -4241,24 +4261,38 @@
     def Filter(self):
         return self._Filter
 
     @Filter.setter
     def Filter(self, Filter):
         self._Filter = Filter
 
+    @property
+    def LogFilter(self):
+        return self._LogFilter
+
+    @LogFilter.setter
+    def LogFilter(self, LogFilter):
+        self._LogFilter = LogFilter
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Order = params.get("Order")
         self._OrderBy = params.get("OrderBy")
         if params.get("Filter") is not None:
             self._Filter = AuditLogFilter()
             self._Filter._deserialize(params.get("Filter"))
+        if params.get("LogFilter") is not None:
+            self._LogFilter = []
+            for item in params.get("LogFilter"):
+                obj = InstanceAuditLogFilters()
+                obj._deserialize(item)
+                self._LogFilter.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -17002,14 +17036,99 @@
 
     def _deserialize(self, params):
         self._Price = params.get("Price")
         self._OriginalPrice = params.get("OriginalPrice")
         self._RequestId = params.get("RequestId")
 
 
+class InstanceAuditLogFilters(AbstractModel):
+    """审计日志搜索过滤器
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Type: 过滤项。目前支持以下搜索条件：
+
+分词搜索：
+sql - SQL语句；
+
+等于、不等于、包含、不包含：
+host - 客户端地址；
+user - 用户名；
+dbName - 数据库名称；
+
+等于、不等于：
+sqlType - SQL类型；
+errCode - 错误码；
+threadId - 线程ID；
+
+范围搜索（时间类型统一为微妙）：
+execTime - 执行时间；
+lockWaitTime - 执行时间；
+ioWaitTime - IO等待时间；
+trxLivingTime - 事物持续时间；
+cpuTime - cpu时间；
+checkRows - 扫描行数；
+affectRows - 影响行数；
+sentRows - 返回行数。
+        :type Type: str
+        :param _Compare: 过滤条件。支持以下条件：
+INC - 包含,
+EXC - 不包含,
+EQS - 等于,
+NEQ - 不等于,
+RA - 范围。
+        :type Compare: str
+        :param _Value: 过滤的值。
+        :type Value: list of str
+        """
+        self._Type = None
+        self._Compare = None
+        self._Value = None
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def Compare(self):
+        return self._Compare
+
+    @Compare.setter
+    def Compare(self, Compare):
+        self._Compare = Compare
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+
+    def _deserialize(self, params):
+        self._Type = params.get("Type")
+        self._Compare = params.get("Compare")
+        self._Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class InstanceInfo(AbstractModel):
     """实例详细信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.934/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.933/README.rst` & `tencentcloud-sdk-python-cdb-3.0.934/README.rst`

 * *Files identical despite different names*

