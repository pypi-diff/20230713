# Comparing `tmp/warrant-python-2.1.0.tar.gz` & `tmp/warrant-python-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warrant-python-2.1.0.tar", last modified: Wed Mar 22 22:42:02 2023, max compression
+gzip compressed data, was "warrant-python-2.2.0.tar", last modified: Thu Jul 13 20:48:16 2023, max compression
```

## Comparing `warrant-python-2.1.0.tar` & `warrant-python-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:42:02.656468 warrant-python-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-22 22:41:51.000000 warrant-python-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-22 22:42:02.652468 warrant-python-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-22 22:41:51.000000 warrant-python-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 22:42:02.656468 warrant-python-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-03-22 22:41:51.000000 warrant-python-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:42:02.652468 warrant-python-2.1.0/warrant/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/authz.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/pricing_tier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-22 22:41:51.000000 warrant-python-2.1.0/warrant/warrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:42:02.652468 warrant-python-2.1.0/warrant_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-22 22:42:02.000000 warrant-python-2.1.0/warrant_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-22 22:42:02.000000 warrant-python-2.1.0/warrant_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 22:42:02.000000 warrant-python-2.1.0/warrant_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-22 22:42:02.000000 warrant-python-2.1.0/warrant_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 22:42:02.000000 warrant-python-2.1.0/warrant_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:16.474620 warrant-python-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 20:48:01.000000 warrant-python-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-13 20:48:16.474620 warrant-python-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 20:48:01.000000 warrant-python-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:48:16.474620 warrant-python-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-13 20:48:01.000000 warrant-python-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:16.474620 warrant-python-2.2.0/warrant/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/authz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/pricing_tier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-13 20:48:01.000000 warrant-python-2.2.0/warrant/warrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:16.474620 warrant-python-2.2.0/warrant_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-13 20:48:16.000000 warrant-python-2.2.0/warrant_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 20:48:16.000000 warrant-python-2.2.0/warrant_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:48:16.000000 warrant-python-2.2.0/warrant_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 20:48:16.000000 warrant-python-2.2.0/warrant_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:48:16.000000 warrant-python-2.2.0/warrant_python.egg-info/top_level.txt
```

### Comparing `warrant-python-2.1.0/LICENSE` & `warrant-python-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/PKG-INFO` & `warrant-python-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrant-python
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python SDK for Warrant
 Home-page: https://github.com/warrant-dev/warrant-python
 Author: Warrant
 Author-email: hello@warrant.dev
 License: Apache Software License (http://www.apache.org/licenses/LICENSE-2.0.txt)
 Project-URL: Bug Tracker, https://github.com/warrant-dev/warrant-python/issues
 Project-URL: Documentation, https://docs.warrant.dev
```

### Comparing `warrant-python-2.1.0/README.md` & `warrant-python-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/setup.py` & `warrant-python-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 DIR = pathlib.Path(__file__).parent
 README = (DIR / "README.md").read_text()
 
 setup(
     name="warrant-python",
-    version="2.1.0",
+    version="2.2.0",
     description="Python SDK for Warrant",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Warrant",
     author_email="hello@warrant.dev",
     url="https://github.com/warrant-dev/warrant-python",
     license="Apache Software License (http://www.apache.org/licenses/LICENSE-2.0.txt)",
```

### Comparing `warrant-python-2.1.0/warrant/__init__.py` & `warrant-python-2.2.0/warrant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 from warrant.permission import Permission
 from warrant.pricing_tier import PricingTier
 from warrant.role import Role
 
 from warrant.user import User
 from warrant.tenant import Tenant
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 api_key = ""
 api_endpoint = "https://api.warrant.dev"
 self_service_dashboard_base_url = "https://self-serve.warrant.dev"
 user_agent = "warrant-python/" + __version__
```

### Comparing `warrant-python-2.1.0/warrant/api_resource.py` & `warrant-python-2.2.0/warrant/api_resource.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/authz.py` & `warrant-python-2.2.0/warrant/authz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import warrant
 from warrant import APIResource
 
 
 class Authz(APIResource):
 
     @classmethod
-    def check(cls, object_type, object_id, relation, subject):
+    def check(cls, object_type, object_id, relation, subject, context={}):
         warrantToCheck = {
             "objectType": object_type,
             "objectId": object_id,
             "relation": relation,
             "subject": {
                 "objectType": subject.object_type,
                 "objectId": subject.object_id,
                 "relation": subject.relation
-            }
+            },
+            "context": context
         }
         payload = {
             "op": "anyOf",
             "warrants": [warrantToCheck]
         }
         json_resp = cls._post(uri="/v2/authorize", json=payload)
         code = json_resp["code"]
```

### Comparing `warrant-python-2.1.0/warrant/feature.py` & `warrant-python-2.2.0/warrant/feature.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/permission.py` & `warrant-python-2.2.0/warrant/permission.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/pricing_tier.py` & `warrant-python-2.2.0/warrant/pricing_tier.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/role.py` & `warrant-python-2.2.0/warrant/role.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/tenant.py` & `warrant-python-2.2.0/warrant/tenant.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/user.py` & `warrant-python-2.2.0/warrant/user.py`

 * *Files identical despite different names*

### Comparing `warrant-python-2.1.0/warrant/warrant.py` & `warrant-python-2.2.0/warrant/warrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,54 +23,58 @@
     def __init__(self, obj):
         self.object_type = obj["objectType"]
         self.object_id = obj["objectId"]
         self.relation = obj["relation"]
         self.subject = obj["subject"]
 
     @classmethod
-    def create(cls, object_type, object_id, relation, subject):
+    def create(cls, object_type, object_id, relation, subject, policy=""):
         payload = {
             "objectType": object_type,
             "objectId": object_id,
             "relation": relation
         }
         if isinstance(subject, Subject):
             payload["subject"] = {
                 "objectType": subject.object_type,
                 "objectId": subject.object_id,
                 "relation": subject.relation
             }
         else:
             raise WarrantException(msg="Invalid type for \'subject\'. Must be of type Subject")
+        if policy != "":
+            payload["policy"] = policy
         cls._post(uri="/v1/warrants", json=payload)
 
     @classmethod
     def query(cls, select, for_clause, where):
         params = {
             "select": select,
             "for": for_clause,
             "where": where,
         }
         return cls._get(uri="/v1/query", params=params, object_hook=Warrant.from_json)
 
     @classmethod
-    def delete(cls, object_type, object_id, relation, subject):
+    def delete(cls, object_type, object_id, relation, subject, policy=""):
         payload = {
             "objectType": object_type,
             "objectId": object_id,
             "relation": relation
         }
         if isinstance(subject, Subject):
             payload["subject"] = {
                 "objectType": subject.object_type,
                 "objectId": subject.object_id,
                 "relation": subject.relation
             }
         else:
             raise WarrantException(msg="Invalid type for \'subject\'. Must be of type Subject")
+        if policy != "":
+            payload["policy"] = policy
         cls._delete(uri="/v1/warrants", json=payload)
 
     """
     JSON serialization/deserialization
     """
     @staticmethod
     def from_json(obj):
```

### Comparing `warrant-python-2.1.0/warrant_python.egg-info/PKG-INFO` & `warrant-python-2.2.0/warrant_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warrant-python
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python SDK for Warrant
 Home-page: https://github.com/warrant-dev/warrant-python
 Author: Warrant
 Author-email: hello@warrant.dev
 License: Apache Software License (http://www.apache.org/licenses/LICENSE-2.0.txt)
 Project-URL: Bug Tracker, https://github.com/warrant-dev/warrant-python/issues
 Project-URL: Documentation, https://docs.warrant.dev
```

