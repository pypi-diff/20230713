# Comparing `tmp/opnsenseapi-0.4.0.tar.gz` & `tmp/opnsenseapi-0.5.0.tar.gz`

## Comparing `opnsenseapi-0.4.0.tar` & `opnsenseapi-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.flake8
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/GITHUB_CHANGELOG.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/cog.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/package.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/opnsenseapi.iml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/opnsense.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/__init__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/unbound.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/__init__.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override_test.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/__init__.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/ifaces/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/ifaces/opnsense.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/README.md
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.flake8
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/GITHUB_CHANGELOG.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/cog.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/package.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/modules.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/opnsenseapi.iml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/__init__.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/opnsense.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/unbound.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/__init__.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/host_override.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/host_override_test.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/models/__init__.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/models/hosts.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/models/hosts_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/ifaces/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/opnsenseapi/ifaces/opnsense.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/README.md
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.5.0/PKG-INFO
```

### Comparing `opnsenseapi-0.4.0/.readthedocs.yaml` & `opnsenseapi-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/CHANGELOG.md` & `opnsenseapi-0.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file. See [conventional commits](https://www.conventionalcommits.org/) for commit guidelines.
 
 - - -
+## 0.5.0 - 2023-07-13
+#### Features
+- Restructured Project - (0a25e0f) - eBeyond
+#### Refactoring
+- Restructured Project - (7882f44) - eBeyond
+
+- - -
+
 ## 0.4.0 - 2023-07-13
 #### Bug Fixes
 - Removed grappa-http due to wrong version - (e396d58) - eBeyond
 - Removed grappa-http due to wrong version - (52dd130) - eBeyond
 - Removed grappa-http due to wrong version - (720e0f1) - eBeyond
 #### Features
 - Restructured Project - (d0bb93c) - eBeyond
```

### Comparing `opnsenseapi-0.4.0/cog.toml` & `opnsenseapi-0.5.0/cog.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/opnsenseapi/opnsense.py` & `opnsenseapi-0.5.0/opnsenseapi/opnsense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 
 import requests
 import urllib3
 from requests.auth import HTTPBasicAuth
 
-from opnsenseapi.core.core import Core
+from opnsenseapi.core.core import Core, _Core
 from opnsenseapi.ifaces.opnsense import _OpnSense
 
 
 class OpnSense(_OpnSense):
     opnsense_address: str
     opnsense_key: str
     opnsense_secret: str
@@ -74,9 +74,9 @@
         print(url)
         r = requests.get(
             url,
             verify=self.verify_cert,
             auth=self.auth)
         return r.text
 
-    def core(self):
+    def core(self) -> _Core:
         return Core(self)
```

### Comparing `opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override.py` & `opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/host_override.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 import json
-import math
 
 from opnsenseapi.core.unbound.settings.models.hosts import Host, MXHost, AHost
 from opnsenseapi.ifaces.opnsense import _OpnSense
 
 
-class HostOverride(object):
+class _HostOverride:
+    def create(self, host: Host):
+        pass
+
+    def read(self, id: str):
+        pass
+
+    def update(self, host: Host):
+        pass
+
+    def delete_by_id(self, id: str):
+        pass
+
+    def delete_by_host(self, host: Host):
+        pass
+
+    def get(self, id):
+        pass
+
+    def list(self):
+        pass
+
+    def search(self):
+        pass
+
+
+class HostOverride(_HostOverride):
     ctrl: _OpnSense
-    module = "unbound"
-    controller = "settings"
+    module: str
+    controller: str
 
-    def __init__(self, ctrl: _OpnSense):
+    def __init__(self, ctrl: _OpnSense, module="unbound", controller="settings"):
         self.ctrl = ctrl
+        self.module = module
+        self.controller = controller
 
     def create(self, host: Host):
         data = host.to_json()
         result = self.ctrl.modifying_request(self.module, self.controller, 'addHostOverride', data=data)
         if result['result'] == "saved":
             host.id = result['uuid']
             return host
@@ -36,24 +63,24 @@
                                              params=[host.id])
         print(f"RES: {result}")
         if result['result'] == "saved":
             return host
         else:
             raise Exception(f"Error updating host: {result}")
 
-    def delete_by_host(self, host: Host):
-        return self.delete_by_id(host.id)
-
     def delete_by_id(self, id: str):
         result = self.ctrl.modifying_request(self.module, self.controller, 'delHostOverride', params=[id])
         if result['result'] == 'deleted':
             return True
         else:
             return False
 
+    def delete_by_host(self, host: Host):
+        return self.delete_by_id(host.id)
+
     def get(self, id):
         return self.read(id)
 
     def list(self):
         result = self.ctrl.non_modifying_request(self.module, self.controller, 'searchHostOverride')
         print(result)
```

### Comparing `opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override_test.py` & `opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/host_override_test.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts.py` & `opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/models/hosts.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts_test.py` & `opnsenseapi-0.5.0/opnsenseapi/core/unbound/settings/models/hosts_test.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/.gitignore` & `opnsenseapi-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/LICENSE` & `opnsenseapi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/pyproject.toml` & `opnsenseapi-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.4.0/PKG-INFO` & `opnsenseapi-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnsenseapi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python API for access the opnsense api
 Project-URL: Documentation, https://opnsenseapi.readthedocs.io/
 Project-URL: Changelog, https://opnsenseapi.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://opnsenseapi.pypa.io/latest/
 Project-URL: History, https://opnsenseapi.pypa.io/dev/history/opnsenseapi/
 Project-URL: Tracker, https://github.com/oss4u/opnsenseapi/issues
 Project-URL: Source, https://github.com/oss4u/opnsenseapi
```

