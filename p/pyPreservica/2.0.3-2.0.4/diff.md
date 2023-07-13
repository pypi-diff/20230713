# Comparing `tmp/pyPreservica-2.0.3.tar.gz` & `tmp/pyPreservica-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-2.0.3.tar", last modified: Tue Jul  4 09:08:45 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.4.tar", last modified: Thu Jul 13 09:22:04 2023, max compression
```

## Comparing `pyPreservica-2.0.3.tar` & `pyPreservica-2.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.160763 pyPreservica-2.0.3/pyPreservica/
--rw-rw-rw-   0        0        0     1084 2023-07-04 08:59:07.000000 pyPreservica-2.0.3/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.3/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.3/pyPreservica/authorityAPI.py
--rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.3/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.3/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.3/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.3/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.3/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.3/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.3/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.3/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:08:45.192005 pyPreservica-2.0.3/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-04 09:08:44.000000 pyPreservica-2.0.3/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 09:08:45.198521 pyPreservica-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-07-03 15:13:51.000000 pyPreservica-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.868092 pyPreservica-2.0.4/pyPreservica/
+-rw-rw-rw-   0        0        0     1085 2023-07-13 09:21:50.000000 pyPreservica-2.0.4/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37810 2023-07-13 09:10:01.000000 pyPreservica-2.0.4/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0     9142 2023-07-04 08:59:07.000000 pyPreservica-2.0.4/pyPreservica/authorityAPI.py
+-rw-rw-rw-   0        0        0    34848 2023-07-03 10:50:28.000000 pyPreservica-2.0.4/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105749 2023-07-05 09:27:42.000000 pyPreservica-2.0.4/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.4/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.4/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.4/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92455 2023-06-06 12:57:35.000000 pyPreservica-2.0.4/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.4/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.4/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:22:04.914955 pyPreservica-2.0.4/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-07-13 09:22:04.000000 pyPreservica-2.0.4/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 09:22:03.000000 pyPreservica-2.0.4/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:22:04.930575 pyPreservica-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-07-13 09:21:50.000000 pyPreservica-2.0.4/setup.py
```

### Comparing `pyPreservica-2.0.3/LICENSE.txt` & `pyPreservica-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/PKG-INFO` & `pyPreservica-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.3/README.md` & `pyPreservica-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/__init__.py` & `pyPreservica-2.0.4/pyPreservica/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-pyPreservica module definition
+pyPreservica package definition
 import API classes, for entity, content, upload, workflows & retention
 
 author:     James Carr
 licence:    Apache License 2.0
 
 """
 from .common import *
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .authorityAPI import AuthorityAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-2.0.3/pyPreservica/adminAPI.py` & `pyPreservica-2.0.4/pyPreservica/adminAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,15 +691,18 @@
                 schema_dict = {}
                 schema_uri = schema.find(f'.//{{{self.admin_ns}}}SchemaUri')
                 name = schema.find(f'.//{{{self.admin_ns}}}Name')
                 description = schema.find(f'.//{{{self.admin_ns}}}Description')
                 aip_id = schema.find(f'.//{{{self.admin_ns}}}ApiId')
                 schema_dict['SchemaUri'] = schema_uri.text
                 schema_dict['Name'] = name.text
-                schema_dict['Description'] = description.text
+                if description is not None:
+                    schema_dict['Description'] = description.text
+                else:
+                    schema_dict['Description'] = ""
                 schema_dict['ApiId'] = aip_id.text
                 results.append(schema_dict)
             return results
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.xml_schemas()
         else:
```

### Comparing `pyPreservica-2.0.3/pyPreservica/authorityAPI.py` & `pyPreservica-2.0.4/pyPreservica/authorityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/common.py` & `pyPreservica-2.0.4/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/contentAPI.py` & `pyPreservica-2.0.4/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/entityAPI.py` & `pyPreservica-2.0.4/pyPreservica/entityAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
 
         :param entity:       The entity with the metadata
         """
 
         for uri, schema in entity.metadata.items():
             yield tuple((str(schema), self.metadata(uri)))
 
-    def metadata_for_entity(self, entity: Entity, schema: str) -> str:
+    def metadata_for_entity(self, entity: Entity, schema: str) -> Union[str, None]:
         """
         Retrieve the first metadata fragment on an entity with a matching schema URI
 
         Returns XML document as a string
 
         :param entity:       The entity with the metadata
         :param schema:       The schema URI
@@ -1019,34 +1019,35 @@
         # if the entity is a lightweight enum version request the full object
         if entity.metadata is None:
             entity = self.entity(entity.entity_type, entity.reference)
 
         for uri, schema_name in entity.metadata.items():
             if schema == schema_name:
                 return self.metadata(uri)
-        return None
+        return
 
     def metadata_tag_for_entity(self, entity: Entity, schema: str, tag: str, isXpath: bool = False) -> str:
         """
         Retrieve the first value of the tag from a metadata template given by schema
 
         Returns XML document as a string
 
         :param isXpath:      True if the tag name is a fully qualified xpath expression
         :param entity:       The entity with the metadata
         :param schema:       The schema URI
         :param tag:          The tag name
         """
 
         xml_doc = self.metadata_for_entity(entity, schema)
-        xml_object = xml.etree.ElementTree.fromstring(xml_doc)
-        if isXpath is False:
-            return xml_object.find(f'.//{{*}}{tag}').text
-        else:
-            return xml_object.find(tag).text
+        if xml_doc:
+            xml_object = xml.etree.ElementTree.fromstring(xml_doc)
+            if isXpath is False:
+                return xml_object.find(f'.//{{*}}{tag}').text
+            else:
+                return xml_object.find(tag).text
 
     def security_tag_sync(self, entity: Entity, new_tag: str):
         """
          Change the security tag for a folder or asset
 
          Returns the updated entity after the security tag has been updated.
```

### Comparing `pyPreservica-2.0.3/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.4/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/opex.py` & `pyPreservica-2.0.4/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/parAPI.py` & `pyPreservica-2.0.4/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.4/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.4/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.4/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.4/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.4/pyPreservica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-2.0.3/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.4/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-2.0.3/setup.py` & `pyPreservica-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="2.0.3",
+    version="2.0.4",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

