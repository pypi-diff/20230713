# Comparing `tmp/tencentcloud-sdk-python-iai-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-iai-3.0.934.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.933.tar", last modified: Wed Jul 12 00:31:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iai-3.0.934.tar", last modified: Thu Jul 13 00:23:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iai-3.0.933.tar` & `tencentcloud-sdk-python-iai-3.0.934.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12105 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49375 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/iai_client.py
--rw-r--r--   0 root         (0) root         (0)   250297 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46159 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/iai_client.py
--rw-r--r--   0 root         (0) root         (0)   236125 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:31:05.000000 tencentcloud-sdk-python-iai-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:31:04.000000 tencentcloud-sdk-python-iai-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12105 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49375 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)   250297 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46159 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/iai_client.py
+-rw-r--r--   0 root         (0) root         (0)   236125 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:23:37.000000 tencentcloud-sdk-python-iai-3.0.934/README.rst
```

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud_sdk_python_iai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud_sdk_python_iai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.933/setup.py` & `tencentcloud-sdk-python-iai-3.0.934/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20200303/models.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20200303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/errorcodes.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/iai_client.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/iai/v20180301/models.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/iai/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iai-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iai-3.0.934/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iai-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-iai-3.0.934/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iai
-Version: 3.0.933
+Version: 3.0.934
 Summary: Tencent Cloud Iai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iai-3.0.933/README.rst` & `tencentcloud-sdk-python-iai-3.0.934/README.rst`

 * *Files identical despite different names*

