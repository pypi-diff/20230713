# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.933.tar", last modified: Wed Jul 12 00:22:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.934.tar", last modified: Thu Jul 13 00:18:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.933.tar` & `tencentcloud-sdk-python-ckafka-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    71620 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)   765151 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-12 00:22:59.000000 tencentcloud-sdk-python-ckafka-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-12 00:22:58.000000 tencentcloud-sdk-python-ckafka-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    71620 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)   766499 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-13 00:18:27.000000 tencentcloud-sdk-python-ckafka-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.934/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -21925,22 +21925,34 @@
         :type Domain: str
         :param _DomainPort: 域名port
 注意：此字段可能返回 null，表示取不到有效值。
         :type DomainPort: int
         :param _DeleteTimestamp: 时间戳
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeleteTimestamp: str
+        :param _Subnet: 子网信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Subnet: str
+        :param _BrokerVipList: 虚拟IP列表(1对1 broker节点)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BrokerVipList: list of VipEntity
+        :param _VpcId: vpc信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
         """
         self._AccessType = None
         self._RouteId = None
         self._VipType = None
         self._VipList = None
         self._Domain = None
         self._DomainPort = None
         self._DeleteTimestamp = None
+        self._Subnet = None
+        self._BrokerVipList = None
+        self._VpcId = None
 
     @property
     def AccessType(self):
         return self._AccessType
 
     @AccessType.setter
     def AccessType(self, AccessType):
@@ -21990,28 +22002,60 @@
     def DeleteTimestamp(self):
         return self._DeleteTimestamp
 
     @DeleteTimestamp.setter
     def DeleteTimestamp(self, DeleteTimestamp):
         self._DeleteTimestamp = DeleteTimestamp
 
+    @property
+    def Subnet(self):
+        return self._Subnet
+
+    @Subnet.setter
+    def Subnet(self, Subnet):
+        self._Subnet = Subnet
+
+    @property
+    def BrokerVipList(self):
+        return self._BrokerVipList
+
+    @BrokerVipList.setter
+    def BrokerVipList(self, BrokerVipList):
+        self._BrokerVipList = BrokerVipList
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
 
     def _deserialize(self, params):
         self._AccessType = params.get("AccessType")
         self._RouteId = params.get("RouteId")
         self._VipType = params.get("VipType")
         if params.get("VipList") is not None:
             self._VipList = []
             for item in params.get("VipList"):
                 obj = VipEntity()
                 obj._deserialize(item)
                 self._VipList.append(obj)
         self._Domain = params.get("Domain")
         self._DomainPort = params.get("DomainPort")
         self._DeleteTimestamp = params.get("DeleteTimestamp")
+        self._Subnet = params.get("Subnet")
+        if params.get("BrokerVipList") is not None:
+            self._BrokerVipList = []
+            for item in params.get("BrokerVipList"):
+                obj = VipEntity()
+                obj._deserialize(item)
+                self._BrokerVipList.append(obj)
+        self._VpcId = params.get("VpcId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.934/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.933/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.934/README.rst`

 * *Files identical despite different names*

