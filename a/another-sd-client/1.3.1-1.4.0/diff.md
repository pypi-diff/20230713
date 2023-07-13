# Comparing `tmp/another_sd_client-1.3.1.tar.gz` & `tmp/another_sd_client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.3.1.tar", max compression
+gzip compressed data, was "another_sd_client-1.4.0.tar", max compression
```

## Comparing `another_sd_client-1.3.1.tar` & `another_sd_client-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     6296 2023-06-16 13:06:33.566820 another_sd_client-1.3.1/README.md
--rw-r--r--   0        0        0      919 2023-06-16 13:06:34.865917 another_sd_client-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 13:06:33.613823 another_sd_client-1.3.1/sdclient/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/client.py
--rw-r--r--   0        0        0     4905 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/requests.py
--rw-r--r--   0        0        0     2697 2023-06-16 13:06:33.568820 another_sd_client-1.3.1/sdclient/responses.py
--rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-07-13 09:41:00.108048 another_sd_client-1.4.0/README.md
+-rw-r--r--   0        0        0      919 2023-07-13 09:41:01.342161 another_sd_client-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 09:41:00.148051 another_sd_client-1.4.0/sdclient/__init__.py
+-rw-r--r--   0        0        0     5018 2023-07-13 09:41:00.109048 another_sd_client-1.4.0/sdclient/client.py
+-rw-r--r--   0        0        0     1017 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/exceptions.py
+-rw-r--r--   0        0        0     4937 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/requests.py
+-rw-r--r--   0        0        0     2697 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/responses.py
+-rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.4.0/PKG-INFO
```

### Comparing `another_sd_client-1.3.1/README.md` & `another_sd_client-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.1/pyproject.toml` & `another_sd_client-1.4.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 
 [tool.poetry]
 name = "another-sd-client"
-version = "1.3.1"
+version = "1.4.0"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
```

### Comparing `another_sd_client-1.3.1/sdclient/client.py` & `another_sd_client-1.4.0/sdclient/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+from pyexpat import ExpatError
 from typing import OrderedDict
 from typing import Tuple
 
 import httpx
 import xmltodict
-
+from httpx import HTTPError
+from httpx import HTTPStatusError
+from httpx import StreamError
+
+from sdclient.exceptions import SDCallError
+from sdclient.exceptions import SDHTTPStatusError
+from sdclient.exceptions import SDParseResponseError
 from sdclient.requests import GetDepartmentRequest
 from sdclient.requests import GetEmploymentRequest
 from sdclient.requests import GetOrganizationRequest
 from sdclient.requests import SDRequest
 from sdclient.responses import GetDepartmentResponse
 from sdclient.responses import GetEmploymentResponse
 from sdclient.responses import GetOrganizationResponse
@@ -42,32 +49,56 @@
         Returns:
             XML response from SD in the form of an OrderedDict
         """
 
         # Get the endpoint name, e.g. "GetEmployment20111201"
         endpoint_name = query_params.get_name() + SDClient.ENDPOINT_SUFFIX
 
-        # TODO: handle request errors properly
-        r = httpx.get(
-            SDClient.BASE_URL + endpoint_name,
-            params=query_params.to_query_params(),
-            auth=(self.username, self.password),
-            timeout=self.timeout,
-        )
-
-        assert 200 <= r.status_code < 300
+        try:
+            response = httpx.get(
+                SDClient.BASE_URL + endpoint_name,
+                params=query_params.to_query_params(),
+                auth=(self.username, self.password),
+                timeout=self.timeout,
+            )
+        except (HTTPError, StreamError) as err:
+            raise SDCallError(
+                "There was a problem calling SD",
+                endpoint_name,
+                query_params,
+            ) from err
+
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as err:
+            raise SDHTTPStatusError(
+                "HTTP error status returned",
+                endpoint_name,
+                query_params,
+                response.status_code,
+                response.text,
+            ) from err
 
         # Nice for debugging
         # import lxml.etree
-        # sd_xml_resp = lxml.etree.XML(r.text.split(">", maxsplit=1)[1])
+        # sd_xml_resp = lxml.etree.XML(response.text.split(">", maxsplit=1)[1])
         # xml = lxml.etree.tostring(sd_xml_resp, pretty_print=True).decode("utf-8")
         # print(xml)
 
-        # TODO: handle XML errors
-        xml_to_ordered_dict = xmltodict.parse(r.text, force_list=xml_force_list)
+        try:
+            xml_to_ordered_dict = xmltodict.parse(
+                response.text, force_list=xml_force_list
+            )
+        except Exception as err:
+            raise SDParseResponseError(
+                "XML response from SD could not be parsed",
+                endpoint_name,
+                query_params,
+            ) from err
+
         root_elem = xml_to_ordered_dict.get(endpoint_name)
 
         return root_elem
 
     def get_department(
         self, query_params: GetDepartmentRequest
     ) -> GetDepartmentResponse:
```

### Comparing `another_sd_client-1.3.1/sdclient/requests.py` & `another_sd_client-1.4.0/sdclient/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     DepartmentNameIndicator: bool = False
     # EmploymentDepartmentIndicator: bool = False
     # PostalAddressIndicator: bool = False
     # ProductionUnitIndicator: bool = False
     UUIDIndicator: bool = False
 
     # TODO: check what is actually required
-    @root_validator
+    @root_validator  # type: ignore
     def check_values(cls, values):
         institution_identifier = values.get("InstitutionIdentifier")
         institution_uuid_identifier = values.get("InstitutionUUIDIdentifier")
         department_identifier = values.get("DepartmentIdentifier")
         department_uuid_identifier = values.get("DepartmentUUIDIdentifier")
 
         if institution_identifier is None and institution_uuid_identifier is None:
@@ -110,15 +110,15 @@
 
     InstitutionIdentifier: str | None = None
     InstitutionUUIDIdentifier: UUID | None = None
     ActivationDate: date
     DeactivationDate: date
     UUIDIndicator: bool = False
 
-    @root_validator
+    @root_validator  # type: ignore
     def check_values(cls, values):
         institution_identifier = values.get("InstitutionIdentifier")
         institution_uuid_identifier = values.get("InstitutionUUIDIdentifier")
         activation_date = values.get("ActivationDate")
         deactivation_date = values.get("DeactivationDate")
 
         # Ensure that exactly one of "InstitutionIdentifier" and
```

### Comparing `another_sd_client-1.3.1/sdclient/responses.py` & `another_sd_client-1.4.0/sdclient/responses.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.3.1/PKG-INFO` & `another_sd_client-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.3.1
+Version: 1.4.0
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

