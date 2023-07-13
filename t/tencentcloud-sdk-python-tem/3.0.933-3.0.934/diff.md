# Comparing `tmp/tencentcloud-sdk-python-tem-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-tem-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.933.tar", last modified: Wed Jul 12 00:41:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.934.tar", last modified: Thu Jul 13 00:35:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tem-3.0.933.tar` & `tencentcloud-sdk-python-tem-3.0.934.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16604 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45873 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   379283 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/__init__.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15756 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   117434 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:41:59.000000 tencentcloud-sdk-python-tem-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16604 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    45873 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   379283 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15756 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   117434 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:35:07.000000 tencentcloud-sdk-python-tem-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-tem-3.0.933/setup.py` & `tencentcloud-sdk-python-tem-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20210701/models.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud/tem/v20201221/models.py` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud/tem/v20201221/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.933/tencentcloud_sdk_python_tem.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.934/tencentcloud_sdk_python_tem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.934/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.933/README.rst` & `tencentcloud-sdk-python-tem-3.0.934/README.rst`

 * *Files identical despite different names*

