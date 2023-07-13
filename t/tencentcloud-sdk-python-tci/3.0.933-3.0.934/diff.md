# Comparing `tmp/tencentcloud-sdk-python-tci-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-tci-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.933.tar", last modified: Wed Jul 12 00:38:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tci-3.0.934.tar", last modified: Thu Jul 13 00:34:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tci-3.0.933.tar` & `tencentcloud-sdk-python-tci-3.0.934.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44023 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/tci_client.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   285108 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:38:14.000000 tencentcloud-sdk-python-tci-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44023 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/tci_client.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   285108 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:34:10.000000 tencentcloud-sdk-python-tci-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-tci-3.0.933/setup.py` & `tencentcloud-sdk-python-tci-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tci-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/tci_client.py` & `tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/tci_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/errorcodes.py` & `tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.933/tencentcloud/tci/v20190318/models.py` & `tencentcloud-sdk-python-tci-3.0.934/tencentcloud/tci/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tci-3.0.933/tencentcloud_sdk_python_tci.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.934/tencentcloud_sdk_python_tci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-tci-3.0.934/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tci
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tci SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tci-3.0.933/README.rst` & `tencentcloud-sdk-python-tci-3.0.934/README.rst`

 * *Files identical despite different names*

