# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.933.tar", last modified: Wed Jul 12 00:29:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.934.tar", last modified: Thu Jul 13 00:22:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.933.tar` & `tencentcloud-sdk-python-essbasic-3.0.934.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53839 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   380671 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53839 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   383583 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5574,28 +5574,88 @@
 
     """
 
     def __init__(self):
         r"""
         :param _CanEditFlow: 是否允许修改合同信息，true-是，false-否
         :type CanEditFlow: bool
+        :param _HideShowFlowName: 是否允许发起合同弹窗隐藏合同名称
+        :type HideShowFlowName: bool
+        :param _HideShowFlowType: 是否允许发起合同弹窗隐藏合同类型
+        :type HideShowFlowType: bool
+        :param _HideShowDeadline: 是否允许发起合同弹窗隐藏合同到期时间
+        :type HideShowDeadline: bool
+        :param _CanSkipAddApprover: 是否允许发起合同步骤跳过指定签署方步骤
+        :type CanSkipAddApprover: bool
+        :param _CustomCreateFlowDescription: 定制化发起合同页合同描述信息
+        :type CustomCreateFlowDescription: str
         """
         self._CanEditFlow = None
+        self._HideShowFlowName = None
+        self._HideShowFlowType = None
+        self._HideShowDeadline = None
+        self._CanSkipAddApprover = None
+        self._CustomCreateFlowDescription = None
 
     @property
     def CanEditFlow(self):
         return self._CanEditFlow
 
     @CanEditFlow.setter
     def CanEditFlow(self, CanEditFlow):
         self._CanEditFlow = CanEditFlow
 
+    @property
+    def HideShowFlowName(self):
+        return self._HideShowFlowName
+
+    @HideShowFlowName.setter
+    def HideShowFlowName(self, HideShowFlowName):
+        self._HideShowFlowName = HideShowFlowName
+
+    @property
+    def HideShowFlowType(self):
+        return self._HideShowFlowType
+
+    @HideShowFlowType.setter
+    def HideShowFlowType(self, HideShowFlowType):
+        self._HideShowFlowType = HideShowFlowType
+
+    @property
+    def HideShowDeadline(self):
+        return self._HideShowDeadline
+
+    @HideShowDeadline.setter
+    def HideShowDeadline(self, HideShowDeadline):
+        self._HideShowDeadline = HideShowDeadline
+
+    @property
+    def CanSkipAddApprover(self):
+        return self._CanSkipAddApprover
+
+    @CanSkipAddApprover.setter
+    def CanSkipAddApprover(self, CanSkipAddApprover):
+        self._CanSkipAddApprover = CanSkipAddApprover
+
+    @property
+    def CustomCreateFlowDescription(self):
+        return self._CustomCreateFlowDescription
+
+    @CustomCreateFlowDescription.setter
+    def CustomCreateFlowDescription(self, CustomCreateFlowDescription):
+        self._CustomCreateFlowDescription = CustomCreateFlowDescription
+
 
     def _deserialize(self, params):
         self._CanEditFlow = params.get("CanEditFlow")
+        self._HideShowFlowName = params.get("HideShowFlowName")
+        self._HideShowFlowType = params.get("HideShowFlowType")
+        self._HideShowDeadline = params.get("HideShowDeadline")
+        self._CanSkipAddApprover = params.get("CanSkipAddApprover")
+        self._CustomCreateFlowDescription = params.get("CustomCreateFlowDescription")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8721,18 +8781,22 @@
         :param _ComponentId: 表单域或控件的ID，跟ComponentName二选一，不能全为空；
 CreateFlowsByTemplates 接口不使用此字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentId: str
         :param _ComponentName: 控件的名字，跟ComponentId二选一，不能全为空
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentName: str
+        :param _LockComponentValue: 是否锁定模版控件值，锁定后无法修改（用于嵌入式发起合同）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LockComponentValue: bool
         """
         self._ComponentValue = None
         self._ComponentId = None
         self._ComponentName = None
+        self._LockComponentValue = None
 
     @property
     def ComponentValue(self):
         return self._ComponentValue
 
     @ComponentValue.setter
     def ComponentValue(self, ComponentValue):
@@ -8750,19 +8814,28 @@
     def ComponentName(self):
         return self._ComponentName
 
     @ComponentName.setter
     def ComponentName(self, ComponentName):
         self._ComponentName = ComponentName
 
+    @property
+    def LockComponentValue(self):
+        return self._LockComponentValue
+
+    @LockComponentValue.setter
+    def LockComponentValue(self, LockComponentValue):
+        self._LockComponentValue = LockComponentValue
+
 
     def _deserialize(self, params):
         self._ComponentValue = params.get("ComponentValue")
         self._ComponentId = params.get("ComponentId")
         self._ComponentName = params.get("ComponentName")
+        self._LockComponentValue = params.get("LockComponentValue")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.934/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.934/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

