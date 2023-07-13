# Comparing `tmp/imerit_ango-1.1.9-py3-none-any.whl.zip` & `tmp/imerit_ango-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9685 bytes, number of entries: 11
+Zip file size: 9781 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/__init__.py
 -rw-r--r--  2.0 unx     1304 b- defN 23-Jul-10 08:52 imerit_ango/plugin_logger.py
--rw-r--r--  2.0 unx     6635 b- defN 23-Jul-10 10:37 imerit_ango/plugins.py
--rw-r--r--  2.0 unx    15198 b- defN 23-Jul-10 12:49 imerit_ango/sdk.py
+-rw-r--r--  2.0 unx     6925 b- defN 23-Jul-12 10:57 imerit_ango/plugins.py
+-rw-r--r--  2.0 unx    16587 b- defN 23-Jul-12 10:54 imerit_ango/sdk.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/models/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Jul-10 08:52 imerit_ango/models/enums.py
 -rw-r--r--  2.0 unx     5452 b- defN 23-Jul-10 08:52 imerit_ango/models/label_category.py
--rw-r--r--  2.0 unx     1940 b- defN 23-Jul-12 10:42 imerit_ango-1.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:42 imerit_ango-1.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-12 10:42 imerit_ango-1.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-12 10:42 imerit_ango-1.1.9.dist-info/RECORD
-11 files, 31616 bytes uncompressed, 8171 bytes compressed:  74.2%
+-rw-r--r--  2.0 unx     1940 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-13 10:52 imerit_ango-1.2.0.dist-info/RECORD
+11 files, 33295 bytes uncompressed, 8267 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imerit_ango/models/enums.py
 Comment: 
 
 Filename: imerit_ango/models/label_category.py
 Comment: 
 
-Filename: imerit_ango-1.1.9.dist-info/METADATA
+Filename: imerit_ango-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: imerit_ango-1.1.9.dist-info/WHEEL
+Filename: imerit_ango-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: imerit_ango-1.1.9.dist-info/top_level.txt
+Filename: imerit_ango-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: imerit_ango-1.1.9.dist-info/RECORD
+Filename: imerit_ango-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imerit_ango/plugins.py

```diff
@@ -73,17 +73,18 @@
     def start(self):
         asyncio.get_event_loop().run_forever()
 
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
-                 host="https://imeritapi.ango.ai"):
+                 host="https://imeritapi.ango.ai", version: str = "v2"):
         super().__init__(id, secret, callback)
         self.host = host
+        self.version = version
 
     def on_plugin(self, data):
         """
         :param data: {project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime = None, tags: List[str] = None}
         :return:
         """
@@ -98,15 +99,19 @@
             completed_at = [datetime.datetime.fromisoformat(data.completed_at[0]),
                             datetime.datetime.fromisoformat(data.completed_at[1])]
         if data.get("updated_at", None):
             updated_at = [datetime.datetime.fromisoformat(data.updated_at[0]),
                           datetime.datetime.fromisoformat(data.updated_at[1])]
 
         try:
-            json_export = sdk.export(project_id, data.get('assignees', None), completed_at=completed_at,
+            if self.version == 'v3':
+                json_export = sdk.exportV3(project_id, batches=data.get('batches', None),
+                                         stage=data.get('stage', None), format="ndjson")
+            else:
+                json_export = sdk.export(project_id, data.get('assignees', None), completed_at=completed_at,
                                      updated_at=updated_at, batches=data.get('batches', None),
                                      stage=data.get('stage', None), format="ndjson")
         except Exception as e:
             logger.error(f"Error calling sdk.export: {e}")
             return
 
         data["jsonExport"] = json_export
```

## imerit_ango/sdk.py

```diff
@@ -309,14 +309,53 @@
                 if format == "ndjson":
                     json_response = self.__generate_ndjson_iterator(content)
                 else:
                     json_response = json.loads(content)
 
         return json_response
 
+    def exportV3(self, project_id: str, batches: List[str] = None, stage: str = None, format: str ="json"):
+
+        params = {
+            'project': project_id,
+            'sendEmail': 'false',
+            'format': format,
+            'includeMetadata': 'true',
+            'includeHistory': 'true',
+            'includeMask': 'true',
+            'includeSegmentationPoints': 'true',
+            'doNotNotify': 'true'
+        }
+
+        if batches:
+            params['batches'] = json.dumps(batches)
+        if stage:
+            params['stage'] = json.dumps(stage)
+
+
+        url = f"{self.host}/v2/exportV3?{urlencode(params)}"
+        headers = {'apikey': self.api_key}
+
+        response = self.session.get(url, headers=headers)
+        response.raise_for_status()  # raises an HTTPError if the response was an HTTP 4xx or 5xx
+
+        link = response.json()['data']['exportPath']
+        filehandle, _ = urllib.request.urlretrieve(link)
+
+        with zipfile.ZipFile(filehandle, 'r') as zip_file_object:
+            first_file = zip_file_object.namelist()[0]
+            with zip_file_object.open(first_file) as file:
+                content = file.read()
+                if format == "ndjson":
+                    json_response = self.__generate_ndjson_iterator(content)
+                else:
+                    json_response = json.loads(content)
+
+        return json_response
+
     def create_label_set(self, project_id: str, tools: List[ToolCategory] = [],
                          classifications: List[ClassificationCategory] = [],
                          relations: List[RelationCategory] = []):
 
         url = "%s/v2/project/%s" % (self.host, project_id)
         headers = {
             'apikey': self.api_key
```

## Comparing `imerit_ango-1.1.9.dist-info/METADATA` & `imerit_ango-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.9
+Version: 1.2.0
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

