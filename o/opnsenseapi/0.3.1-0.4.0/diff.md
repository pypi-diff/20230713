# Comparing `tmp/opnsenseapi-0.3.1.tar.gz` & `tmp/opnsenseapi-0.4.0.tar.gz`

## Comparing `opnsenseapi-0.3.1.tar` & `opnsenseapi-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,35 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.flake8
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/GITHUB_CHANGELOG.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/cog.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/package.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/opnsenseapi.iml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/ifaces/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/ifaces/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/__init__.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/host_override.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/host_override_test.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/README.md
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.flake8
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/GITHUB_CHANGELOG.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/cog.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/package.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/opnsenseapi.iml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/opnsense.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/__init__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/unbound.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/__init__.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override_test.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/__init__.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/models/hosts_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/ifaces/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/opnsenseapi/ifaces/opnsense.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/README.md
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.4.0/PKG-INFO
```

### Comparing `opnsenseapi-0.3.1/.readthedocs.yaml` & `opnsenseapi-0.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.1/CHANGELOG.md` & `opnsenseapi-0.4.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 All notable changes to this project will be documented in this file. See [conventional commits](https://www.conventionalcommits.org/) for commit guidelines.
 
 - - -
+## 0.4.0 - 2023-07-13
+#### Bug Fixes
+- Removed grappa-http due to wrong version - (e396d58) - eBeyond
+- Removed grappa-http due to wrong version - (52dd130) - eBeyond
+- Removed grappa-http due to wrong version - (720e0f1) - eBeyond
+#### Features
+- Restructured Project - (d0bb93c) - eBeyond
+
+- - -
+
 ## 0.3.1 - 2023-07-12
 #### Bug Fixes
 - issue with mxprio in host overrides - (5a2bf2f) - eBeyond
 - Fixed numeric error while using mxprio - (d9d3e77) - eBeyond
 
 - - -
```

### Comparing `opnsenseapi-0.3.1/cog.toml` & `opnsenseapi-0.4.0/cog.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.1/opnsenseapi/opnsense.py` & `opnsenseapi-0.4.0/opnsenseapi/opnsense.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 
 import requests
 import urllib3
 from requests.auth import HTTPBasicAuth
 
-import opnsenseapi.unbound.host_override
+from opnsenseapi.core.core import Core
 from opnsenseapi.ifaces.opnsense import _OpnSense
 
 
 class OpnSense(_OpnSense):
     opnsense_address: str
     opnsense_key: str
     opnsense_secret: str
@@ -72,11 +72,11 @@
         else:
             url = f"{self.opnsense_address}/api/{module}/{controller}/{command}"
         print(url)
         r = requests.get(
             url,
             verify=self.verify_cert,
             auth=self.auth)
-        return r.json()
+        return r.text
 
-    def unbound_host_overrides(self):
-        return opnsenseapi.unbound.host_override.HostOverride(self)
+    def core(self):
+        return Core(self)
```

### Comparing `opnsenseapi-0.3.1/opnsenseapi/unbound/host_override_test.py` & `opnsenseapi-0.4.0/opnsenseapi/core/unbound/settings/host_override_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,83 @@
 import json
 import unittest
+import pook
 
-from opnsenseapi.ifaces.opnsense import _OpnSense
-from opnsenseapi.unbound.host_override import HostOverride, Host
+from opnsenseapi.core.unbound.settings.host_override import HostOverride
+from opnsenseapi.opnsense import OpnSense
 
 
 class HostOverrideTest(unittest.TestCase):
-    def test_host_to_json(self):
-        class MockValidator(_OpnSense):
-            pass
-        mocker = MockValidator
-        ho = HostOverride(mocker)
-        expected = Host(
-            enabled=True,
-            hostname="hostname",
-            domain="domain",
-            rr="A",
-            server="10.10.10.10",
-            description="descr"
-        )
-        test = json.dumps({
+    def test_get_ahost_success(self):
+        response = {
             "host": {
                 "enabled": "1",
-                "hostname": "hostname",
-                "domain": "domain",
-                "rr": "A",
+                "hostname": "test01",
+                "domain": "test.de",
+                "rr": {
+                    "A": {
+                        "value": "A (IPv4 address)",
+                        "selected": 1
+                    },
+                    "AAAA": {
+                        "value": "AAAA (IPv6 address)",
+                        "selected": 0
+                    },
+                    "MX": {
+                        "value": "MX (Mail server)",
+                        "selected": 0
+                    }
+                },
                 "mxprio": "",
                 "mx": "",
                 "server": "10.10.10.10",
-                "description": "descr"
+                "description": "My Test Host"
             }
-        }, indent=2)
-        result = ho.create_host_from_json(json.loads(test))
-
+        }
+        pook.on()
+        pook.get('https://fw:8443/api/unbound/settings/getHostOverride/existing', reply=200,
+                 response_headers={'Server': 'nginx'},
+                 response_json=response)
+        os = OpnSense(opnsense_address="https://fw:8443", opnsense_secret="os-secret", opnsense_key="os-key")
+        overr = HostOverride(os)
+        result = overr.get("existing")
         print(result)
-        print(expected)
-
-        self.assertEqual(result, expected)  # add assertion here
 
-    def test_json_to_host(self):
-        class MockValidator(_OpnSense):
-            pass
-        mocker = MockValidator
-        ho = HostOverride(mocker)
-        test = Host(id="abc",
-                    enabled=True,
-                    hostname="hostname",
-                    domain="domain",
-                    rr="A",
-                    server="10.10.10.10",
-                    description="descr")
-        expected = json.dumps({
+    def test_get_ahost_404(self):
+        response = {
             "host": {
                 "enabled": "1",
-                "hostname": "hostname",
-                "domain": "domain",
-                "rr": "A",
+                "hostname": "test01",
+                "domain": "test.de",
+                "rr": {
+                    "A": {
+                        "value": "A (IPv4 address)",
+                        "selected": 1
+                    },
+                    "AAAA": {
+                        "value": "AAAA (IPv6 address)",
+                        "selected": 0
+                    },
+                    "MX": {
+                        "value": "MX (Mail server)",
+                        "selected": 0
+                    }
+                },
                 "mxprio": "",
                 "mx": "",
                 "server": "10.10.10.10",
-                "description": "descr"
+                "description": "My Test Host"
             }
-        })
-        result = ho.create_json_from_host(test)
-        self.assertEqual(sorted(json.loads(result)), sorted(json.loads(expected)))  # add assertion here
+        }
+        pook.on()
+        pook.get('https://fw:8443/api/unbound/settings/getHostOverride/abc', reply=404,
+                 response_headers={'Server': 'nginx'},
+                 response_json=response)
+        os = OpnSense(opnsense_address="https://fw:8443", opnsense_secret="os-secret",
+                                           opnsense_key="os-key")
+        overr = HostOverride(os)
+        result = overr.get("abc")
+        print(result)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `opnsenseapi-0.3.1/.gitignore` & `opnsenseapi-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.1/LICENSE` & `opnsenseapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.1/pyproject.toml` & `opnsenseapi-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.1/PKG-INFO` & `opnsenseapi-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnsenseapi
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python API for access the opnsense api
 Project-URL: Documentation, https://opnsenseapi.readthedocs.io/
 Project-URL: Changelog, https://opnsenseapi.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://opnsenseapi.pypa.io/latest/
 Project-URL: History, https://opnsenseapi.pypa.io/dev/history/opnsenseapi/
 Project-URL: Tracker, https://github.com/oss4u/opnsenseapi/issues
 Project-URL: Source, https://github.com/oss4u/opnsenseapi
```

