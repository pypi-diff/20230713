# Comparing `tmp/target_s3_delta-0.0.8.tar.gz` & `tmp/target_s3_delta-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_s3_delta-0.0.8.tar", max compression
+gzip compressed data, was "target_s3_delta-0.0.9.tar", max compression
```

## Comparing `target_s3_delta-0.0.8.tar` & `target_s3_delta-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.8/README.md
--rw-r--r--   0        0        0     1051 2023-06-23 11:17:02.763208 target_s3_delta-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.8/target_s3_delta/__init__.py
--rw-r--r--   0        0        0      104 2023-06-22 12:08:20.986818 target_s3_delta-0.0.8/target_s3_delta/common.py
--rw-r--r--   0        0        0     5947 2023-06-23 09:41:08.021757 target_s3_delta-0.0.8/target_s3_delta/sinks.py
--rw-r--r--   0        0        0     4316 2023-06-23 11:16:37.192304 target_s3_delta-0.0.8/target_s3_delta/target.py
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 target_s3_delta-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.9/README.md
+-rw-r--r--   0        0        0     1051 2023-07-06 08:14:57.954154 target_s3_delta-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.9/target_s3_delta/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-22 12:08:20.986818 target_s3_delta-0.0.9/target_s3_delta/common.py
+-rw-r--r--   0        0        0     4319 2023-07-06 08:13:34.191998 target_s3_delta-0.0.9/target_s3_delta/sinks.py
+-rw-r--r--   0        0        0     4316 2023-07-06 08:09:42.875447 target_s3_delta-0.0.9/target_s3_delta/target.py
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 target_s3_delta-0.0.9/PKG-INFO
```

### Comparing `target_s3_delta-0.0.8/pyproject.toml` & `target_s3_delta-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-s3-delta"
-version = "0.0.8"
+version = "0.0.9"
 description = "`target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["resul yurttakalan"]
 keywords = [
     "ELT",
     "s3-delta",
 ]
```

### Comparing `target_s3_delta-0.0.8/target_s3_delta/sinks.py` & `target_s3_delta-0.0.9/target_s3_delta/sinks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """s3-delta target sink class, which handles writing streams."""
 
 from __future__ import annotations
 
 import os
-import time
 from typing import Dict, Optional
 
-from dateutil import parser
 from singer_sdk import PluginBase
-from singer_sdk.helpers._typing import (
-    DatetimeErrorTreatmentEnum,
-    get_datelike_property_type,
-    handle_invalid_timestamp_in_record,
-)
+from singer_sdk.helpers._typing import DatetimeErrorTreatmentEnum
 from singer_sdk.sinks import BatchSink
 import pandas as pd
 
 from target_s3_delta.common import ExtractMode
 
-NOT_PROPER_DATETIME_FORMAT = "0000-00-00 00:00:00"
 TEMP_DATA_DIRECTORY = "/tmp/meltano_temp_data/"
 MAX_SIZE_DEFAULT = 50000
 
 
 class S3DeltaSink(BatchSink):
     """s3-delta target sink class."""
 
     replication_configs: Optional[Dict] = None
 
+    @property
+    def datetime_error_treatment(self) -> DatetimeErrorTreatmentEnum:
+        return DatetimeErrorTreatmentEnum.NULL
+
     def __init__(
         self,
         target: PluginBase,
         stream_name: str,
         schema: dict,
         key_properties: list[str] | None,
     ) -> None:
@@ -95,60 +92,16 @@
             context["records"] = []
 
         if self.is_duplicate_replication(record):
             # Since singer returns at least one last record in incremental cases, we're truncating it.
             # https://www.stitchdata.com/docs/replication/replication-methods/key-based-incremental
             return
 
-        for key in record:
-            date_val = record[key]
-            if date_val == NOT_PROPER_DATETIME_FORMAT:
-                record[key] = None
-
         context["records"].append(record)
 
-    def _parse_timestamps_in_record(
-        self,
-        record: dict,
-        schema: dict,
-        treatment: DatetimeErrorTreatmentEnum,
-    ) -> None:
-        """Parse strings to datetime.datetime values, repairing or erroring on failure.
-
-        Attempts to parse every field that is of type date/datetime/time. If its value
-        is out of range, repair logic will be driven by the `treatment` input arg:
-        MAX, NULL, or ERROR.
-
-        Args:
-            record: Individual record in the stream.
-            schema:
-            treatment:
-        """
-        for key in record:
-            datelike_type = get_datelike_property_type(schema["properties"][key])
-            if datelike_type:
-                date_val = record[key]
-                try:
-                    if record[key] is not None:
-                        if date_val == NOT_PROPER_DATETIME_FORMAT:
-                            record[key] = None
-                        else:
-                            date_val = parser.parse(date_val)
-                except parser.ParserError as ex:
-                    date_val = handle_invalid_timestamp_in_record(
-                        record,
-                        [key],
-                        date_val,
-                        datelike_type,
-                        ex,
-                        treatment,
-                        self.logger,
-                    )
-                record[key] = date_val
-
     def start_batch(self, context: dict) -> None:
         """Start a batch.
 
         Developers may optionally add additional markers to the `context` dict,
         which is unique to this batch.
 
         Args:
```

### Comparing `target_s3_delta-0.0.8/target_s3_delta/target.py` & `target_s3_delta-0.0.9/target_s3_delta/target.py`

 * *Files identical despite different names*

### Comparing `target_s3_delta-0.0.8/PKG-INFO` & `target_s3_delta-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-s3-delta
-Version: 0.0.8
+Version: 0.0.9
 Summary: `target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,s3-delta
 Author: resul yurttakalan
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

