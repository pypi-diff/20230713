# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.933.tar", last modified: Wed Jul 12 00:41:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.934.tar", last modified: Thu Jul 13 00:34:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.933.tar` & `tencentcloud-sdk-python-tdmq-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111089 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   661043 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-12 00:41:48.000000 tencentcloud-sdk-python-tdmq-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111089 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   663304 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:34:58.000000 tencentcloud-sdk-python-tdmq-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 00:34:57.000000 tencentcloud-sdk-python-tdmq-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5281,20 +5281,24 @@
         :param _RoleName: 角色名称
         :type RoleName: str
         :param _Token: 角色token
         :type Token: str
         :param _Remark: 备注说明
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
+        :param _EnvironmentRoleSets: 批量绑定名字空间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnvironmentRoleSets: list of EnvironmentRoleSet
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._RoleName = None
         self._Token = None
         self._Remark = None
+        self._EnvironmentRoleSets = None
         self._RequestId = None
 
     @property
     def RoleName(self):
         return self._RoleName
 
     @RoleName.setter
@@ -5314,26 +5318,40 @@
         return self._Remark
 
     @Remark.setter
     def Remark(self, Remark):
         self._Remark = Remark
 
     @property
+    def EnvironmentRoleSets(self):
+        return self._EnvironmentRoleSets
+
+    @EnvironmentRoleSets.setter
+    def EnvironmentRoleSets(self, EnvironmentRoleSets):
+        self._EnvironmentRoleSets = EnvironmentRoleSets
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RoleName = params.get("RoleName")
         self._Token = params.get("Token")
         self._Remark = params.get("Remark")
+        if params.get("EnvironmentRoleSets") is not None:
+            self._EnvironmentRoleSets = []
+            for item in params.get("EnvironmentRoleSets"):
+                obj = EnvironmentRoleSet()
+                obj._deserialize(item)
+                self._EnvironmentRoleSets.append(obj)
         self._RequestId = params.get("RequestId")
 
 
 class CreateSubscriptionRequest(AbstractModel):
     """CreateSubscription请求参数结构体
 
     """
@@ -13496,14 +13514,62 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EnvironmentRoleSet(AbstractModel):
+    """批量绑定名字空间和角色权限关系
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _EnvironmentId: 需要绑定的命名空间Id，不重复且存在资源
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnvironmentId: str
+        :param _Permissions: 名字空间需要绑定的权限，枚举为 "consume" "produce" 组合，但是不为空
+
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Permissions: list of str
+        """
+        self._EnvironmentId = None
+        self._Permissions = None
+
+    @property
+    def EnvironmentId(self):
+        return self._EnvironmentId
+
+    @EnvironmentId.setter
+    def EnvironmentId(self, EnvironmentId):
+        self._EnvironmentId = EnvironmentId
+
+    @property
+    def Permissions(self):
+        return self._Permissions
+
+    @Permissions.setter
+    def Permissions(self, Permissions):
+        self._Permissions = Permissions
+
+
+    def _deserialize(self, params):
+        self._EnvironmentId = params.get("EnvironmentId")
+        self._Permissions = params.get("Permissions")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ExchangeQuota(AbstractModel):
     """exchange使用配额信息
 
     """
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.934/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.933/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.934/README.rst`

 * *Files identical despite different names*

