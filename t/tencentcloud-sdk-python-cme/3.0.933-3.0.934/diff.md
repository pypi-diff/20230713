# Comparing `tmp/tencentcloud-sdk-python-cme-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-cme-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.933.tar", last modified: Wed Jul 12 00:23:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cme-3.0.934.tar", last modified: Thu Jul 13 00:19:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cme-3.0.933.tar` & `tencentcloud-sdk-python-cme-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/
--rw-r--r--   0 root         (0) root         (0)    55254 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/cme_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   444352 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:23:32.000000 tencentcloud-sdk-python-cme-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:23:31.000000 tencentcloud-sdk-python-cme-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/
+-rw-r--r--   0 root         (0) root         (0)    55251 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/cme_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   444358 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:19:01.000000 tencentcloud-sdk-python-cme-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-cme-3.0.933/setup.py` & `tencentcloud-sdk-python-cme-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cme-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/cme_client.py` & `tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/cme_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateLink(self, request):
-        """创建媒体链接或分类路径链接，将源资源信息链接到目标。
+        """创建媒体链接或分类路径链接，将资源信息链接到目标。
 
         :param request: Request instance for CreateLink.
         :type request: :class:`tencentcloud.cme.v20191029.models.CreateLinkRequest`
         :rtype: :class:`tencentcloud.cme.v20191029.models.CreateLinkResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/errorcodes.py` & `tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cme-3.0.933/tencentcloud/cme/v20191029/models.py` & `tencentcloud-sdk-python-cme-3.0.934/tencentcloud/cme/v20191029/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4687,15 +4687,15 @@
         :type AspectRatio: str
         :param _CoverData: 视频封面图片文件（如 jpeg, png 等）进行 Base64 编码后的字符串，仅支持 gif、jpeg、png 三种图片格式，原图片文件不能超过2 M大 小。
         :type CoverData: str
         :param _CMEExportInfo: 导出的多媒体创作引擎媒体信息。当导出目标为 CME 时必填。
         :type CMEExportInfo: :class:`tencentcloud.cme.v20191029.models.CMEExportInfo`
         :param _VODExportInfo: 导出的云点播媒资信息。当导出目标为 VOD 时必填。
         :type VODExportInfo: :class:`tencentcloud.cme.v20191029.models.VODExportInfo`
-        :param _Operator: 操作者。如不填，默认为 `cmeid_system`，表示平台管理员操作，无权限限制。如果指定操作者，轨道数据中使的媒资该操作者需要拥有使用权限。
+        :param _Operator: 操作者。如不填，默认为 `cmeid_system`，表示平台管理员操作，无权限限制。如果指定操作者，轨道数据中使用的媒资该操作者需要拥有使用权限。
         :type Operator: str
         """
         self._Platform = None
         self._Definition = None
         self._ExportDestination = None
         self._TrackData = None
         self._AspectRatio = None
@@ -6427,15 +6427,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _MaterialId: 媒体 Id。
         :type MaterialId: str
-        :param _PreProcessTaskId: 媒体文预处理任务 ID，如果未指定发起预处理任务则为空。
+        :param _PreProcessTaskId: 媒体文件预处理任务 ID，如果未指定发起预处理任务则为空。
         :type PreProcessTaskId: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._MaterialId = None
         self._PreProcessTaskId = None
         self._RequestId = None
@@ -8367,15 +8367,15 @@
         :type DestinationInfos: list of MediaCastDestinationInfo
         :param _OutputMediaSetting: 输出媒体配置。
         :type OutputMediaSetting: :class:`tencentcloud.cme.v20191029.models.MediaCastOutputMediaSetting`
         :param _PlaySetting: 播放参数。
         :type PlaySetting: :class:`tencentcloud.cme.v20191029.models.MediaCastPlaySetting`
         :param _StartTime: 项目启动时间。采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _StopTime: 项目结束时间。采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。如果项目还在运行中，改字段为空。
+        :param _StopTime: 项目结束时间。采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。如果项目还在运行中，该字段为空。
         :type StopTime: str
         """
         self._Status = None
         self._SourceInfos = None
         self._DestinationInfos = None
         self._OutputMediaSetting = None
         self._PlaySetting = None
@@ -9590,15 +9590,15 @@
         :type MemberId: str
         :param _Remark: 成员备注，长度不能超过15个字符。
         :type Remark: str
         :param _Role: 成员角色，可取值有：
 <li>Admin：团队管理员；</li>
 <li>Member：普通成员。</li>
         :type Role: str
-        :param _Operator: 操作者。如不填，默认为 `cmeid_system`，表示平台管理员操作，可以个改任意团队成员的信息。如果指定操作者，则操作者必须为团队的管理员或者所有者。
+        :param _Operator: 操作者。如不填，默认为 `cmeid_system`，表示平台管理员操作，可以修改任意团队成员的信息。如果指定操作者，则操作者必须为团队的管理员或者所有者。
         :type Operator: str
         """
         self._Platform = None
         self._TeamId = None
         self._MemberId = None
         self._Remark = None
         self._Role = None
```

### Comparing `tencentcloud-sdk-python-cme-3.0.933/tencentcloud_sdk_python_cme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.934/tencentcloud_sdk_python_cme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-cme-3.0.934/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cme
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cme-3.0.933/README.rst` & `tencentcloud-sdk-python-cme-3.0.934/README.rst`

 * *Files identical despite different names*

