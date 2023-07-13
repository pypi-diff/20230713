# Comparing `tmp/contact_magic-0.5.2.tar.gz` & `tmp/contact_magic-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.2.tar", max compression
+gzip compressed data, was "contact_magic-0.5.3.tar", max compression
```

## Comparing `contact_magic-0.5.2.tar` & `contact_magic-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.2/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.2/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.2/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.2/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.5.2/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.2/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.2/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.2/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-08 20:52:26.946536 contact_magic-0.5.2/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.2/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.2/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.2/contact_magic/logger.py
--rw-r--r--   0        0        0    15182 2023-07-08 21:41:34.642770 contact_magic-0.5.2/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.2/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.2/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.2/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.2/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.2/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.2/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.2/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.2/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.2/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-07-09 10:38:49.448262 contact_magic-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.3/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.3/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.3/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.3/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5418 2023-07-13 11:03:11.215506 contact_magic-0.5.3/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2394 2023-06-27 14:36:54.461469 contact_magic-0.5.3/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-08 21:49:20.995044 contact_magic-0.5.3/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.3/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-13 10:14:40.612229 contact_magic-0.5.3/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1678 2023-07-08 23:06:56.717869 contact_magic-0.5.3/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.3/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.3/contact_magic/logger.py
+-rw-r--r--   0        0        0    16259 2023-07-13 11:03:11.410196 contact_magic-0.5.3/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.3/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.3/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.3/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.3/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.3/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.3/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.3/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.3/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.3/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-13 11:03:28.052391 contact_magic-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.3/PKG-INFO
```

### Comparing `contact_magic-0.5.2/README.md` & `contact_magic-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/asyncio.py` & `contact_magic-0.5.3/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/conf/settings.py` & `contact_magic-0.5.3/contact_magic/conf/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,19 @@
         default={},
     )
     SENTENCE_WIZARD_OPTIONS: dict = Field(
         description="Mapping where the keys are the scraper names "
         "and the values are a dict of additional scraper options to pass.",
         default={},
     )
+    ENABLE_SCRAPER_REUSE: bool = Field(
+        description="This setting determines whether a contact can "
+        "have multiple personalized sentences from the same scraper.",
+        default=False,
+    )
 
     @validator("TIMEZONE")
     def validate_timezone(cls, value):
         timezones = pytz.all_timezones_set
         if value not in timezones:
             value = "America/New_York"
         return value
```

### Comparing `contact_magic-0.5.2/contact_magic/dict_utils.py` & `contact_magic-0.5.3/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/helpers.py` & `contact_magic-0.5.3/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.3/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.3/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/integrations/sheets.py` & `contact_magic-0.5.3/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/models.py` & `contact_magic-0.5.3/contact_magic/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -276,22 +276,39 @@
 
     col_name: str = Field(
         description="The column name you want for the datapoint.",
         example="Personalization1",
     )
     sentence_wizards: list[SentenceWizard]
     keys_added: set = set()
+    successful_scraper_name: str = ""
+
+    @property
+    def has_successful_sentence(self):
+        return len(self.successful_scraper_name) > 0
 
     @property
     def get_col_name_as_source(self) -> str:
         return f"source__{self.col_name}"
 
-    async def build_datapoint(self, row: DataRow, keys_to_delete: set = None):
+    async def build_datapoint(
+        self, row: DataRow, keys_to_delete: set = None, wizards_to_remove: set = None
+    ):
         keys_to_delete = keys_to_delete or set()
-        for scraper in self.sentence_wizards:
+        wizards_to_remove = wizards_to_remove or set()
+        if wizards_to_remove:
+            wizards = [
+                wizard
+                for wizard in self.sentence_wizards
+                if wizard.scraper_name not in wizards_to_remove
+            ]
+        else:
+            wizards = self.sentence_wizards
+        # remove any wizards for this row that have been used.
+        for scraper in wizards:
             logger.info(
                 "processing_row",
                 row_number=row.index,
                 scraper_name=scraper.scraper_name,
                 premise_id=scraper.premise_id or get_id_from_url(scraper.premise_url),
                 column_name=self.col_name,
                 status="STARTING",
@@ -301,14 +318,16 @@
                 self.col_name,
                 self.get_col_name_as_source,
                 keys_to_delete=keys_to_delete,
             )
             for key in scraper.added_key_names:
                 self.keys_added.add(key)
             if did_succeed:
+                if scraper.scraper_name != "FALLBACK":
+                    self.successful_scraper_name = scraper.scraper_name
                 logger.info(
                     "processing_row",
                     row_number=row.index,
                     scraper_name=scraper.scraper_name,
                     premise_id=scraper.premise_id
                     or get_id_from_url(scraper.premise_url),
                     column_name=self.col_name,
@@ -401,21 +420,33 @@
 
     def process_data_rows(self, data: list[DataRow]) -> list[DataRow]:
         """
         Process DataRows async.
         :param data:
         :return:
         """
-        return asyncio.run(do_bulk([(self.build_row, {"row": row}) for row in data]))
+        return asyncio.run(
+            do_bulk(
+                [(self.build_row, {"row": row}) for row in data],
+                max_workers=SETTINGS.MAX_WORKERS,
+            )
+        )
 
     async def build_row(self, row: DataRow):
         """
         Iterate over all personalization datapoints and their
         allowed scrapers to extend a row of contact data
         with enrichment and personalized sentences.
         """
         keys_to_delete = set()
+        wizards_to_remove = set()
+
         for datapoint in self.datapoints:
-            row = await datapoint.build_datapoint(row, keys_to_delete=keys_to_delete)
+            row = await datapoint.build_datapoint(
+                row, keys_to_delete=keys_to_delete, wizards_to_remove=wizards_to_remove
+            )
+            if SETTINGS.ENABLE_SCRAPER_REUSE is False:
+                if datapoint.has_successful_sentence:
+                    wizards_to_remove.add(datapoint.successful_scraper_name)
             for key in datapoint.keys_added:
                 keys_to_delete.add(key)
         return row
```

### Comparing `contact_magic-0.5.2/contact_magic/preprocessors.py` & `contact_magic-0.5.3/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/scripts/agency.py` & `contact_magic-0.5.3/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.5.3/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.3/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.5.3/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.3/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/contact_magic/utils.py` & `contact_magic-0.5.3/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.2/pyproject.toml` & `contact_magic-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.2"
+version = "0.5.3"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.2/PKG-INFO` & `contact_magic-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.2
+Version: 0.5.3
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

