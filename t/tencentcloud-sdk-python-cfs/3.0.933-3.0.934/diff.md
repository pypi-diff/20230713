# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.933.tar", last modified: Wed Jul 12 00:22:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.934.tar", last modified: Thu Jul 13 00:17:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.933.tar` & `tencentcloud-sdk-python-cfs-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    39796 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193044 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   193136 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/setup.py` & `tencentcloud-sdk-python-cfs-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Protocols: 协议与售卖详情
         :type Protocols: list of AvailableProtoStatus
-        :param _Type: 存储类型。返回值中 SD 为标准型存储、HP 为性能型存储
+        :param _Type: 存储类型。返回值中 SD 为通用标准型存储， HP为通用性能型存储， TB为Turbo标准型， TP 为Turbo性能型。
         :type Type: str
         :param _Prepayment: 是否支持预付费。返回值中 true 为支持、false 为不支持
         :type Prepayment: bool
         """
         self._Protocols = None
         self._Type = None
         self._Prepayment = None
@@ -5114,15 +5114,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FileSystemId: 文件系统Id
         :type FileSystemId: str
-        :param _TargetCapacity: 扩容的目标容量
+        :param _TargetCapacity: 扩容的目标容量（单位GiB）
         :type TargetCapacity: int
         """
         self._FileSystemId = None
         self._TargetCapacity = None
 
     @property
     def FileSystemId(self):
@@ -5159,15 +5159,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FileSystemId: 文件系统Id
         :type FileSystemId: str
-        :param _TargetCapacity: 扩容的目标容量
+        :param _TargetCapacity: 扩容的目标容量（单位GiB）
         :type TargetCapacity: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._FileSystemId = None
         self._TargetCapacity = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.934/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.933/README.rst` & `tencentcloud-sdk-python-cfs-3.0.934/README.rst`

 * *Files identical despite different names*

