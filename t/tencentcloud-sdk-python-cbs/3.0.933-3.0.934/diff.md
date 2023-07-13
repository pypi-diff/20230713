# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.933.tar", last modified: Wed Jul 12 00:21:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.934.tar", last modified: Thu Jul 13 00:17:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.933.tar` & `tencentcloud-sdk-python-cbs-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)    53328 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   239960 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:21:29.000000 tencentcloud-sdk-python-cbs-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    53328 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   239960 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:06.000000 tencentcloud-sdk-python-cbs-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.934/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/setup.py` & `tencentcloud-sdk-python-cbs-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.934/tencentcloud/cbs/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.934/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.933/README.rst` & `tencentcloud-sdk-python-cbs-3.0.934/README.rst`

 * *Files identical despite different names*

