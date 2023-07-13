# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.932.tar", last modified: Tue Jul 11 00:41:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.934.tar", last modified: Thu Jul 13 00:20:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.932.tar` & `tencentcloud-sdk-python-cynosdb-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    11292 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   679294 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   118494 2023-07-11 00:41:03.000000 tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   118494 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11292 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   684792 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:20:05.000000 tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.934/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.932
+Version: 3.0.934
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.932
+Version: 3.0.934
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.934/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.932'
+__version__ = '3.0.934'
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,22 +837,40 @@
         :type DBName: str
         :param _Sql: SQL语句。
         :type Sql: str
         :param _Host: 客户端地址。
         :type Host: str
         :param _User: 用户名。
         :type User: str
-        :param _ExecTime: 执行时间。
+        :param _ExecTime: 执行时间，微秒。
         :type ExecTime: int
-        :param _Timestamp: 时间戳。
+        :param _Timestamp: 时间。
         :type Timestamp: str
-        :param _SentRows: 发送行数。
+        :param _SentRows: 返回行数。
         :type SentRows: int
         :param _ThreadId: 执行线程ID。
         :type ThreadId: int
+        :param _CheckRows: 扫描行数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CheckRows: int
+        :param _CpuTime: cpu执行时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CpuTime: float
+        :param _IoWaitTime: IO等待时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IoWaitTime: int
+        :param _LockWaitTime: 锁等待时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LockWaitTime: int
+        :param _TrxLivingTime: 事物持续等待时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TrxLivingTime: int
+        :param _NsTime: 开始时间，与timestamp构成一个精确到纳秒的时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NsTime: int
         """
         self._AffectRows = None
         self._ErrCode = None
         self._SqlType = None
         self._TableName = None
         self._InstanceName = None
         self._PolicyName = None
@@ -860,14 +878,20 @@
         self._Sql = None
         self._Host = None
         self._User = None
         self._ExecTime = None
         self._Timestamp = None
         self._SentRows = None
         self._ThreadId = None
+        self._CheckRows = None
+        self._CpuTime = None
+        self._IoWaitTime = None
+        self._LockWaitTime = None
+        self._TrxLivingTime = None
+        self._NsTime = None
 
     @property
     def AffectRows(self):
         return self._AffectRows
 
     @AffectRows.setter
     def AffectRows(self, AffectRows):
@@ -973,14 +997,62 @@
     def ThreadId(self):
         return self._ThreadId
 
     @ThreadId.setter
     def ThreadId(self, ThreadId):
         self._ThreadId = ThreadId
 
+    @property
+    def CheckRows(self):
+        return self._CheckRows
+
+    @CheckRows.setter
+    def CheckRows(self, CheckRows):
+        self._CheckRows = CheckRows
+
+    @property
+    def CpuTime(self):
+        return self._CpuTime
+
+    @CpuTime.setter
+    def CpuTime(self, CpuTime):
+        self._CpuTime = CpuTime
+
+    @property
+    def IoWaitTime(self):
+        return self._IoWaitTime
+
+    @IoWaitTime.setter
+    def IoWaitTime(self, IoWaitTime):
+        self._IoWaitTime = IoWaitTime
+
+    @property
+    def LockWaitTime(self):
+        return self._LockWaitTime
+
+    @LockWaitTime.setter
+    def LockWaitTime(self, LockWaitTime):
+        self._LockWaitTime = LockWaitTime
+
+    @property
+    def TrxLivingTime(self):
+        return self._TrxLivingTime
+
+    @TrxLivingTime.setter
+    def TrxLivingTime(self, TrxLivingTime):
+        self._TrxLivingTime = TrxLivingTime
+
+    @property
+    def NsTime(self):
+        return self._NsTime
+
+    @NsTime.setter
+    def NsTime(self, NsTime):
+        self._NsTime = NsTime
+
 
     def _deserialize(self, params):
         self._AffectRows = params.get("AffectRows")
         self._ErrCode = params.get("ErrCode")
         self._SqlType = params.get("SqlType")
         self._TableName = params.get("TableName")
         self._InstanceName = params.get("InstanceName")
@@ -989,14 +1061,20 @@
         self._Sql = params.get("Sql")
         self._Host = params.get("Host")
         self._User = params.get("User")
         self._ExecTime = params.get("ExecTime")
         self._Timestamp = params.get("Timestamp")
         self._SentRows = params.get("SentRows")
         self._ThreadId = params.get("ThreadId")
+        self._CheckRows = params.get("CheckRows")
+        self._CpuTime = params.get("CpuTime")
+        self._IoWaitTime = params.get("IoWaitTime")
+        self._LockWaitTime = params.get("LockWaitTime")
+        self._TrxLivingTime = params.get("TrxLivingTime")
+        self._NsTime = params.get("NsTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2563,23 +2641,26 @@
         :param _Order: 排序方式。支持值包括："ASC" - 升序，"DESC" - 降序。
         :type Order: str
         :param _OrderBy: 排序字段。支持值包括：
 "timestamp" - 时间戳；
 "affectRows" - 影响行数；
 "execTime" - 执行时间。
         :type OrderBy: str
-        :param _Filter: 过滤条件。可按设置的过滤条件过滤日志。
+        :param _Filter: 已废弃。
         :type Filter: :class:`tencentcloud.cynosdb.v20190107.models.AuditLogFilter`
+        :param _LogFilter: 审计日志过滤条件
+        :type LogFilter: list of InstanceAuditLogFilter
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
@@ -2621,24 +2702,38 @@
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
+                obj = InstanceAuditLogFilter()
+                obj._deserialize(item)
+                self._LogFilter.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8501,29 +8596,32 @@
         :param _Order: 排序方式。支持值包括："ASC" - 升序，"DESC" - 降序。
         :type Order: str
         :param _OrderBy: 排序字段。支持值包括：
 "timestamp" - 时间戳；
 "affectRows" - 影响行数；
 "execTime" - 执行时间。
         :type OrderBy: str
-        :param _Filter: 过滤条件。可按设置的过滤条件过滤日志。
+        :param _Filter: 已废弃。
         :type Filter: :class:`tencentcloud.cynosdb.v20190107.models.AuditLogFilter`
         :param _Limit: 分页参数，单次返回的数据条数。默认值为100，最大值为100。
         :type Limit: int
         :param _Offset: 分页偏移量。
         :type Offset: int
+        :param _LogFilter: 审计日志过滤条件。
+        :type LogFilter: list of InstanceAuditLogFilter
         """
         self._InstanceId = None
         self._StartTime = None
         self._EndTime = None
         self._Order = None
         self._OrderBy = None
         self._Filter = None
         self._Limit = None
         self._Offset = None
+        self._LogFilter = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -8581,26 +8679,40 @@
     def Offset(self):
         return self._Offset
 
     @Offset.setter
     def Offset(self, Offset):
         self._Offset = Offset
 
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
         self._Limit = params.get("Limit")
         self._Offset = params.get("Offset")
+        if params.get("LogFilter") is not None:
+            self._LogFilter = []
+            for item in params.get("LogFilter"):
+                obj = InstanceAuditLogFilter()
+                obj._deserialize(item)
+                self._LogFilter.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -14296,14 +14408,100 @@
                 obj._deserialize(item)
                 self._Prices.append(obj)
         self._InstanceRealTotalPrice = params.get("InstanceRealTotalPrice")
         self._StorageRealTotalPrice = params.get("StorageRealTotalPrice")
         self._RequestId = params.get("RequestId")
 
 
+class InstanceAuditLogFilter(AbstractModel):
+    """审计日志搜索条件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Type: 过滤项。支持以下搜索条件:
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
+
+        :type Type: str
+        :param _Compare: 过滤条件。支持以下选项:
+INC - 包含,
+EXC - 不包含,
+EQS - 等于,
+NEQ - 不等于,
+RA - 范围.
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
 class InstanceAuditRule(AbstractModel):
     """实例的审计规则详情，DescribeAuditRuleWithInstanceIds接口的出参。
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.932/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.934/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

