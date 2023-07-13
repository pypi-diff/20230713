# Comparing `tmp/papertronics-sdk-0.0.35.tar.gz` & `tmp/papertronics-sdk-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.35.tar", last modified: Wed Jul 12 08:46:40 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.36.tar", last modified: Thu Jul 13 12:45:52 2023, max compression
```

## Comparing `papertronics-sdk-0.0.35.tar` & `papertronics-sdk-0.0.36.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-12 08:46:40.494350 papertronics-sdk-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.486349 papertronics-sdk-0.0.35/papertronics_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/status_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/station_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/user_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 08:46:40.494350 papertronics-sdk-0.0.35/setup.cfg
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.823402 papertronics-sdk-0.0.36/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.36/LICENSE
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      971 2023-07-13 12:45:52.823402 papertronics-sdk-0.0.36/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      521 2023-07-11 11:10:18.000000 papertronics-sdk-0.0.36/README.md
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.819402 papertronics-sdk-0.0.36/papertronics_sdk/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.36/papertronics_sdk/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.819402 papertronics-sdk-0.0.36/papertronics_sdk/lab/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     6179 2023-07-13 12:45:42.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/admin_client.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1561 2023-07-11 10:45:50.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/base_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.819402 papertronics-sdk-0.0.36/papertronics_sdk/lab/exceptions/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/exceptions/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      383 2023-07-11 11:01:32.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/exceptions/status_exception.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.823402 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/config.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/database.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/generic.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/models/station_protocol.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9450 2023-07-12 08:45:23.000000 papertronics-sdk-0.0.36/papertronics_sdk/lab/user_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-13 12:45:52.819402 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      971 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      842 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-13 12:45:52.000000 papertronics-sdk-0.0.36/papertronics_sdk.egg-info/zip-safe
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.36/pyproject.toml
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-13 12:45:52.823402 papertronics-sdk-0.0.36/setup.cfg
```

### Comparing `papertronics-sdk-0.0.35/PKG-INFO` & `papertronics-sdk-0.0.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.35
+Version: 0.0.36
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.35/README.md` & `papertronics-sdk-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/admin_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 
     def login_user(self, user_id: uuid.UUID) -> str:
         response = self.post(f"/admin/auth/token",
                              headers={"Authorization": f"Bearer {self.token}"},
                              params={"user_id": user_id})
         return response.json().get("access_token")
 
+    def login_device(self, user_id: uuid.UUID, device_id: uuid.UUID) -> str:
+        response = self.post(f"/admin/auth/device",
+                             headers={"Authorization": f"Bearer {self.token}"},
+                             params={"user_id": user_id, "device_id": device_id})
+        return response.json().get("access_token")
+
     def get_users(self, user_id: Optional[uuid.UUID] = None) -> Union[List[UserModel], UserModel]:
         params = {}
         if user_id:
             params["user_id"] = user_id
         response = self.get(f"/admin/user",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params=params)
```

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/base_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.36/papertronics_sdk/lab/user_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.36/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.35
+Version: 0.0.36
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.35/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.36/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.35/setup.cfg` & `papertronics-sdk-0.0.36/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.35
+version = 0.0.36
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

