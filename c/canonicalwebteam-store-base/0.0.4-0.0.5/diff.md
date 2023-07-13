# Comparing `tmp/canonicalwebteam_store_base-0.0.4.tar.gz` & `tmp/canonicalwebteam_store_base-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_base-0.0.4.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_base-0.0.5.tar", max compression
```

## Comparing `canonicalwebteam_store_base-0.0.4.tar` & `canonicalwebteam_store_base-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/__init__.py
--rw-r--r--   0        0        0     1424 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/app.py
--rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/__init__.py
--rw-r--r--   0        0        0      385 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/authentication.py
--rw-r--r--   0        0        0     1656 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/logic.py
--rw-r--r--   0        0        0     3723 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/views.py
--rw-r--r--   0        0        0    27069 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/data/licenses.json
--rw-r--r--   0        0        0     2745 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/handlers.py
--rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/__init__.py
--rw-r--r--   0        0        0    10518 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/logic.py
--rw-r--r--   0        0        0     2665 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/views.py
--rw-r--r--   0        0        0      201 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/sample_blueprint/views.py
--rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/__init__.py
--rw-r--r--   0        0        0     1094 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/config.py
--rw-r--r--   0        0        0      166 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/constants.py
--rw-r--r--   0        0        0      433 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/decorators.py
--rw-r--r--   0        0        0       61 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/extensions.py
--rw-r--r--   0        0        0     4608 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/helpers.py
--rw-r--r--   0        0        0       25 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/templates/storebase.html
--rw-r--r--   0        0        0     1050 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1304 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/__init__.py
+-rw-r--r--   0        0        0     1424 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/app.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/authentication.py
+-rw-r--r--   0        0        0     1656 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/logic.py
+-rw-r--r--   0        0        0     3723 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/views.py
+-rw-r--r--   0        0        0    27069 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/data/licenses.json
+-rw-r--r--   0        0        0     2745 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/handlers.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/__init__.py
+-rw-r--r--   0        0        0    11998 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/logic.py
+-rw-r--r--   0        0        0     2665 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/views.py
+-rw-r--r--   0        0        0      201 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/sample_blueprint/views.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/config.py
+-rw-r--r--   0        0        0      166 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/constants.py
+-rw-r--r--   0        0        0      433 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/decorators.py
+-rw-r--r--   0        0        0       61 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/extensions.py
+-rw-r--r--   0        0        0     4608 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/helpers.py
+-rw-r--r--   0        0        0       25 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/templates/storebase.html
+-rw-r--r--   0        0        0     1050 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.5/PKG-INFO
```

### Comparing `canonicalwebteam_store_base-0.0.4/LICENSE` & `canonicalwebteam_store_base-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/README.md` & `canonicalwebteam_store_base-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/app.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/logic.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/logic.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/views.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/data/licenses.json` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/data/licenses.json`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/handlers.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/handlers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/logic.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import datetime
+import re
+
+import yaml
 
 import talisker
 from flask import make_response
 from typing import List, Dict, TypedDict, Any
 
 from canonicalwebteam.store_api.exceptions import StoreApiError
 
@@ -34,29 +37,50 @@
     store = store_api(talisker.requests.get_session())
     packages = store.find(fields=fields).get("results", [])
     response = make_response({"packages": packages})
     response.cache_control.max_age = 3600
     return response.json
 
 
+def get_bundle_charms(charm_apps):
+    result = []
+
+    if charm_apps:
+        for app_name, data in charm_apps.items():
+            # Charm names could be with the old prefix/suffix
+            # Like: cs:~charmed-osm/mariadb-k8s-35
+            name = data["charm"]
+            if name.startswith("cs:") or name.startswith("ch:"):
+                name = re.match(r"(?:cs:|ch:)(?:.+/)?(\S*?)(?:-\d+)?$", name)[
+                    1
+                ]
+
+            charm = {"title": format_slug(name), "name": name}
+
+            result.append(charm)
+
+    return result
+
+
 def parse_package_for_card(
-    package: Dict[str, Any], store_name: str
+    package: Dict[str, Any], store_name: str, store_api: Any
 ) -> Package:
     """
     Parses a package (snap, charm, or bundle) and returns the formatted package
     based on the given card schema.
 
     :param: package (Dict[str, Any]): The package to be parsed.
     :returns: a dictionary containing the formatted package.
 
     note:
         - This function has to be refactored to be more generic,
         so we won't have to check for the package type before parsing.
 
     """
+    store = store_api(talisker.requests.get_session())
     resp = {
         "package": {
             "description": "",
             "display_name": "",
             "icon_url": "",
             "name": "",
             "platforms": [],
@@ -76,20 +100,42 @@
         resp["package"]["name"] = package.get("name", "")
         resp["package"]["description"] = result.get("summary", "").split(".")[
             0
         ]
         resp["package"]["display_name"] = result.get(
             "title", format_slug(package.get("name", ""))
         )
-        resp["package"]["platforms"] = result.get("deployable-on", [])
         resp["publisher"]["display_name"] = publisher.get("display-name", "")
         resp["publisher"]["validation"] = publisher.get("validation", "")
         resp["categories"] = result.get("categories", [])
         resp["package"]["icon_url"] = helpers.get_icon(result.get("media", []))
 
+        platforms = result.get("platforms", [])
+        if platforms:
+            resp["package"]["platforms"] = platforms
+        else:
+            resp["package"]["platforms"] = ["vm"]
+
+        if resp["package"]["type"] == "bundle":
+            name = package["name"]
+            default_release = store.get_item_details(
+                name, fields=["default-release"]
+            )
+            bundle_yaml = default_release["default-release"]["revision"][
+                "bundle-yaml"
+            ]
+
+            bundle_details = yaml.load(bundle_yaml, Loader=yaml.FullLoader)
+            bundle_charms = get_bundle_charms(
+                bundle_details.get(
+                    "applications", bundle_details.get("services", [])
+                )
+            )
+            resp["charms"] = bundle_charms
+
     if store_name.startswith("snapcraft"):
         snap = package.get("snap", {})
         publisher = snap.get("publisher", {})
         resp["package"]["description"] = snap.get("summary", "").split(".")[0]
         resp["package"]["display_name"] = snap.get("title", "")
         resp["package"]["type"] = "snap"
         resp["package"]["name"] = package.get("name", "")
@@ -162,24 +208,28 @@
 
     packages = fetch_packages(store, fields).get("packages", [])
     total_pages = -(len(packages) // -size)
 
     if filters:
         parsed_packages = []
         for package in packages:
-            parsed_packages.append(parse_package_for_card(package, store_name))
+            parsed_packages.append(
+                parse_package_for_card(package, store_name, store)
+            )
         filtered_packages = filter_packages(parsed_packages, filters)
         total_pages = -(len(filtered_packages) // -size)
         res = paginate(filtered_packages, page, size, total_pages)
     else:
         total_pages = -(len(packages) // -size)
         packages_per_page = paginate(packages, page, size, total_pages)
         parsed_packages = []
         for package in packages_per_page:
-            parsed_packages.append(parse_package_for_card(package, store_name))
+            parsed_packages.append(
+                parse_package_for_card(package, store_name, store)
+            )
         res = parsed_packages
 
     return {"packages": res, "total_pages": total_pages}
 
 
 def filter_packages(
     packages: List[Package], filter_params: Dict[str, List[str]]
```

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/views.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/config.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/config.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/helpers.py` & `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.4/pyproject.toml` & `canonicalwebteam_store_base-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canonicalwebteam-store-base"
-version = "0.0.4"
+version = "0.0.5"
 description = "An application base for all stores"
 authors = ["Canonical Webteam <webteam@canonical.com>"]
 license = "GPL3"
 readme = "README.md"
 packages = [{include = "canonicalwebteam"}]
 
 [tool.poetry.dependencies]
```

### Comparing `canonicalwebteam_store_base-0.0.4/PKG-INFO` & `canonicalwebteam_store_base-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam-store-base
-Version: 0.0.4
+Version: 0.0.5
 Summary: An application base for all stores
 License: GPL3
 Author: Canonical Webteam
 Author-email: webteam@canonical.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

