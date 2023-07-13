# Comparing `tmp/blockbax_sdk-0.0.8.tar.gz` & `tmp/blockbax_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockbax_sdk-0.0.8.tar", max compression
+gzip compressed data, was "blockbax_sdk-0.0.9.tar", max compression
```

## Comparing `blockbax_sdk-0.0.8.tar` & `blockbax_sdk-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/LICENSE
--rw-r--r--   0        0        0      144 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/README.md
--rw-r--r--   0        0        0     1810 2023-02-08 09:07:36.032035 blockbax_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      632 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/__init__.py
--rw-r--r--   0        0        0      101 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/client/__init__.py
--rw-r--r--   0        0        0       47 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/client/api/__init__.py
--rw-r--r--   0        0        0    17068 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/client/api/api.py
--rw-r--r--   0        0        0     4992 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/client/api/api_utils.py
--rw-r--r--   0        0        0    28139 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/client/http_client.py
--rw-r--r--   0        0        0     1092 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/errors.py
--rw-r--r--   0        0        0      932 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/__init__.py
--rw-r--r--   0        0        0     1179 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/ingestion.py
--rw-r--r--   0        0        0     1499 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/ingestion_collection.py
--rw-r--r--   0        0        0     3662 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/ingestions_utils.py
--rw-r--r--   0        0        0     3080 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/measurement.py
--rw-r--r--   0        0        0     1901 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/metric.py
--rw-r--r--   0        0        0     4507 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/property_type.py
--rw-r--r--   0        0        0     7009 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/property_value.py
--rw-r--r--   0        0        0     1263 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/series.py
--rw-r--r--   0        0        0     5385 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/subject.py
--rw-r--r--   0        0        0     2812 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/models/subject_type.py
--rw-r--r--   0        0        0     2496 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/types.py
--rw-r--r--   0        0        0      103 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/util/__init__.py
--rw-r--r--   0        0        0     3498 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/util/convertions.py
--rw-r--r--   0        0        0      562 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/util/deprecated.py
--rw-r--r--   0        0        0     5337 2023-02-08 09:07:22.044306 blockbax_sdk-0.0.8/src/blockbax_sdk/util/validation.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 blockbax_sdk-0.0.8/setup.py
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 blockbax_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-13 14:48:29.017187 blockbax_sdk-0.0.9/LICENSE
+-rw-r--r--   0        0        0      144 2023-07-13 14:48:29.017187 blockbax_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0     1810 2023-07-13 14:48:44.113315 blockbax_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      632 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/__init__.py
+-rw-r--r--   0        0        0    17107 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/api.py
+-rw-r--r--   0        0        0     4992 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/api_utils.py
+-rw-r--r--   0        0        0     3465 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/readme.md
+-rw-r--r--   0        0        0    28411 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/client/http_client.py
+-rw-r--r--   0        0        0     1092 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/errors.py
+-rw-r--r--   0        0        0      933 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/__init__.py
+-rw-r--r--   0        0        0     2644 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/ingestion.py
+-rw-r--r--   0        0        0     1628 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/ingestion_collection.py
+-rw-r--r--   0        0        0     4599 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/ingestions_utils.py
+-rw-r--r--   0        0        0     3956 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/measurement.py
+-rw-r--r--   0        0        0     1902 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/metric.py
+-rw-r--r--   0        0        0     4507 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/property_type.py
+-rw-r--r--   0        0        0     7009 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/property_value.py
+-rw-r--r--   0        0        0     1635 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/series.py
+-rw-r--r--   0        0        0     5395 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/subject.py
+-rw-r--r--   0        0        0     2812 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/models/subject_type.py
+-rw-r--r--   0        0        0     3148 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/types.py
+-rw-r--r--   0        0        0      103 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/util/__init__.py
+-rw-r--r--   0        0        0     3498 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/util/convertions.py
+-rw-r--r--   0        0        0      562 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/util/deprecated.py
+-rw-r--r--   0        0        0     5785 2023-07-13 14:48:29.021187 blockbax_sdk-0.0.9/src/blockbax_sdk/util/validation.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 blockbax_sdk-0.0.9/PKG-INFO
```

### Comparing `blockbax_sdk-0.0.8/LICENSE` & `blockbax_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/pyproject.toml` & `blockbax_sdk-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blockbax-sdk"
-version = "0.0.8"
+version = "0.0.9"
 description = "Blockbax Python SDK"
 authors = ["Blockbax <development@blockbax.com>"]
 maintainers = ["Blockbax <development@blockbax.com>"]
 readme = "README.md"
 homepage = "https://blockbax.com/docs/integrations/python-sdk/"
 documentation = "https://blockbax.com/docs/python-sdk/"
 keywords = [
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/__init__.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/client/api/api.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Dict, Generator, List, Optional, cast
 
 import logging
 
+
 log = logging.getLogger(__name__)
 
 import json
 import math
 import platform
 import sys
 
@@ -13,14 +14,15 @@
 import httpx
 from tenacity import Retrying, TryAgain, RetryCallState
 from tenacity.wait import wait_exponential
 from tenacity.stop import stop_after_attempt
 
 from blockbax_sdk import __version__
 from . import api_utils
+from ...models.series import SeriesRequest
 
 
 class BlockbaxAuth(httpx.Auth):
     def __init__(self, token: str):
         self.token = token
 
     # Override
@@ -260,15 +262,14 @@
         self,
         name: str,
         external_id: str,
         data_type: str,
         predefined_values: bool = False,
         values: List[dict] = [],
     ):
-
         body = {
             "name": name,
             "externalId": external_id,
             "dataType": data_type,
             "predefinedValues": predefined_values,
             "values": values,
         }
@@ -280,15 +281,14 @@
         property_type_id: str,
         name: str,
         external_id: str,
         data_type: str,
         predefined_values=False,
         values=[],
     ):
-
         body = {
             "name": name,
             "externalId": external_id,
             "dataType": data_type,
             "predefinedValues": predefined_values,
             "values": values,
         }
@@ -353,23 +353,25 @@
 
     def get_subject(self, subject_id: str) -> Optional[dict]:
         return self.get(endpoint=f"{self.subjects_endpoint}/{subject_id}")
 
     def get_subjects(
         self,
         name: Optional[str] = None,
-        subject_ids: List[str] = None,
+        subject_ids: Optional[List[str]] = None,
         subject_type_ids: Optional[list] = None,
+        subject_ids_mode: Optional[str] = None,
         subject_external_id: Optional[str] = None,
         property_value_ids: Optional[str] = None,
     ) -> list:
         params = {
             "name": name,
             "subjectIds": subject_ids,
             "subjectTypeIds": subject_type_ids,
+            "subjectIdsMode": subject_ids_mode,
             "externalId": subject_external_id,
             "propertyValueIds": property_value_ids,
         }
         return self.search(endpoint=self.subjects_endpoint, params=params)
 
     def create_subject(
         self,
@@ -514,11 +516,10 @@
             "fromDate": from_date,
             "toDate": to_date,
             "size": size,
             "order": order,
         }
         return self.get(endpoint=self.measurements_endpoint, params=params)
 
-    def send_measurements(self, series: List[dict], auto_create_subjects: bool = False):
-        body = {"autoCreateSubjects": auto_create_subjects, "series": series}
-        response = self.post(endpoint=self.measurements_endpoint, data=body)
+    def send_measurements(self, series: SeriesRequest):
+        response = self.post(endpoint=self.measurements_endpoint, data=series)
         return response
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/client/api/api_utils.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/client/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/client/http_client.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/client/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             name [required]:
                 The name of the subject type.
             parent_id [optional, default=None]:
                 The ID of the parent subject type of this subject type.
             primary_location [optional, default=None ]:
                 The primary location metric or property type of this subject type, for displaying the location of subjects on the map.
             property_types [optional, default=None ]:
-                List of property type dictionary’s associated with this subject type.
+                List of property type dictionary's associated with this subject type.
 
         Returns: `SubjectType`
         """
         # 'parent_id' will be deprecated in the next sdk version
         if parent_id is not None:
             deprecated.deprecation_warning(
                 "For creating subject types the argument 'parent_id' will be deprecated in the next version of the Blockbax SDK"
@@ -448,16 +448,17 @@
         self.__api.delete_metric(metric_id=id_)
 
     # Methods to create, update, delete and get subjects.
 
     def get_subjects(
         self,
         name: Optional[str] = None,
-        subject_ids: List[str] = None,
+        subject_ids: Optional[List[str]] = None,
         subject_external_id: Optional[str] = None,
+        subject_ids_mode: Optional[str] = None,
         subject_type_ids: Optional[List[str]] = None,
         property_value_ids: Optional[Union[Tuple[str], List[str], str]] = None,
     ) -> List[models.Subject]:
         """Gets subjects, optionally with arguments for filtering.
 
         Arguments:
             name: Filter subjects by name.
@@ -474,14 +475,15 @@
         property_value_ids = convertions.convert_property_value_ids_to_query_filter(
             property_value_ids
         )
 
         subject_responses = self.__api.get_subjects(
             name=name,
             subject_ids=subject_ids,
+            subject_ids_mode=subject_ids_mode,
             subject_external_id=subject_external_id,
             subject_type_ids=subject_type_ids,
             property_value_ids=property_value_ids,
         )
 
         subject_list = []
         for subject_response in subject_responses:
@@ -628,18 +630,19 @@
         self.__api.delete_subject(subject_id=id_)
 
     # Methods to queue, send and get measurements
 
     def queue_measurement(
         self,
         ingestion_id: str,
-        date: Union[datetime.datetime, int, str],
-        number: Optional[Union[decimal.Decimal, Number]] = None,
-        location: Optional[Dict[str, Union[decimal.Decimal, Number, str]]] = None,
+        date: Optional[types.AnyDate],
+        number: Optional[types.AnyNumber] = None,
+        location: Optional[types.LocationLike] = None,
         text: Optional[str] = None,
+        generate_date: bool = False,
     ):
         """Queues measurements to send.
 
         Arguments:
             ingestion_id [required]:
                 Ingestion ID
             date [required]:
@@ -647,21 +650,28 @@
             number [optional, default=None]:
                 Decimal number, must be filled if location = None.
             location [optional, default=None]:
                 Location dictionary, must be filled if number = None.
 
         Returns: `None`
         """
-        if not self.__ingestions[ingestion_id]:
-            self.__ingestions[ingestion_id] = models.Ingestion(id=ingestion_id)
+        if date is None and generate_date:
+            date = datetime.datetime.utcnow()
+
         new_measurement = models.measurement.new(
-            date=date, number=number, location=location, text=text
+            date=date,
+            number=number,
+            location=location,
+            text=text,
         )
         if new_measurement is not None:
-            self.__ingestions[ingestion_id].add_measurement(new_measurement)
+            self.__ingestions.add(
+                ingestion_id=ingestion_id,
+                measurement=new_measurement,
+            )
 
     def send_measurements(
         self,
         ingestion_ids: Optional[List[str]] = None,
         auto_create_subjects: bool = False,
     ):
         """Sends queued measurements.
@@ -672,30 +682,34 @@
             auto_create_subjects [optional, default=False]:
                 Automatically creates a subject for its external ID derived from ingestionId if the subject does not exist (i.e. for the ingestion ID MyCar$Location a subject with external ID MyCar will be created if the metric with external ID Location can be linked to exactly one subject type).
             reset_on_success [optional, default=True]:
                 Option to remove the measurements on success, default will always remove measurements after they have been send
 
         Returns: `None`
         """
+
+        if auto_create_subjects:
+            deprecated.deprecation_warning(
+                "For sending measurements the argument 'auto_create_subjects' will be deprecated in the next version of the Blockbax SDK, to use the auto create feature please see the inbound connector settings."
+            )
+
         if ingestion_ids is None:
             ingestion_ids = []
-        for series_to_send in self.__ingestions.create_series_to_send(
-            ingestion_ids=ingestion_ids,
-            subjects=self.get_subjects(),
-            auto_create_subjects=auto_create_subjects,
+        for series_batch in self.__ingestions.create_series_to_send(
+            ingestion_ids=ingestion_ids
         ):
-            if series_to_send != []:
-                self.__api.send_measurements(
-                    series=series_to_send, auto_create_subjects=auto_create_subjects
-                )
-                if len(ingestion_ids) > 0:
-                    for ingestion_id in ingestion_ids:
-                        self.__ingestions[ingestion_id].measurements.clear()
-                else:
-                    self.__ingestions.clear_all()
+            self.__api.send_measurements(series=series_batch)
+
+        if len(ingestion_ids) > 0:
+            for ingestion_id in ingestion_ids:
+                ingestion = self.__ingestions[ingestion_id]
+                if ingestion is not None:
+                    ingestion.measurements.clear()
+        else:
+            self.__ingestions.clear_all()
 
     def get_measurements(
         self,
         subject_ids: list = [],
         metric_ids: list = [],
         from_date: Union[datetime.datetime, int, str] = None,
         to_date: Union[datetime.datetime, int, str] = None,
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/errors.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/__init__.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .ingestion import Ingestion
 from .ingestion_collection import IngestionCollection
+
 from .series import Series
 from .metric import Metric
 from .subject import Subject
 from .property_type import PropertyType
 from .subject_type import SubjectType
 from .property_value import (
     PropertyValue,
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/ingestion_collection.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/ingestion_collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-from typing import Dict, List, Optional
+from typing import Dict, Iterable, List, Optional
 
+from . import Ingestion
+from . import measurement
 from . import ingestions_utils
-from . import ingestion
-from . import subject
+
+from .series import SeriesRequest
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class IngestionCollection:
-    __ingestions: Dict[str, ingestion.Ingestion]
+    __ingestions: Dict[str, Ingestion]
 
     def __init__(self):
         self.__ingestions = {}
 
-    def __getitem__(self, ingestion_id: str) -> ingestion.Ingestion:
+    def __getitem__(self, ingestion_id: str) -> Optional[Ingestion]:
         return self.__ingestions.get(ingestion_id)
 
-    def __setitem__(self, ingestion_id: str, ingestion: ingestion.Ingestion):
+    def __setitem__(self, ingestion_id: str, ingestion: Ingestion):
         self.__ingestions[ingestion_id] = ingestion
 
+    def __contains__(self, ingestion_id: str) -> bool:
+        return ingestion_id in self.__ingestions
+
+    def add(self, ingestion_id: str, measurement: measurement.Measurement) -> None:
+        if ingestion_id not in self.__ingestions:
+            self.__ingestions[ingestion_id] = Ingestion(id=ingestion_id)
+        self.__ingestions[ingestion_id].add_measurement(measurement)
+
     def get_all_ids(self) -> List[str]:
         return list(self.__ingestions.keys())
 
     def create_series_to_send(
         self,
-        subjects: List[subject.Subject],
-        auto_create_subjects: bool,
-        ingestion_ids: Optional[List[str]] = [],
-    ) -> List:
-        if ingestion_ids:
-            ingestions_to_send = (
-                self.__ingestions[ingestion_id]
-                for ingestion_id in ingestion_ids
-                if ingestion_id in self.__ingestions
-            )
-        else:
-            ingestions_to_send = (
-                ingestion for _, ingestion in self.__ingestions.items()
-            )
+        ingestion_ids: Optional[List[str]] = None,
+    ) -> Iterable[SeriesRequest]:
+        ingestions_to_send: List[Ingestion] = [
+            ingestion
+            for ingestion_id, ingestion in self.__ingestions.items()
+            if ingestion_ids is None or ingestion_id in ingestion_ids
+        ]
 
-        return ingestions_utils.create_series_batches(
+        yield from ingestions_utils.create_series_batches(
             ingestions=ingestions_to_send,
-            subjects=subjects,
-            auto_create_subjects=auto_create_subjects,
         )
 
     def clear_all(self):
-        for _, ingestion in self.__ingestions.items():
+        for ingestion in self.__ingestions.values():
             ingestion.clear()
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/metric.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/metric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from blockbax_sdk.util import convertions
+from typing import Optional
+from ..util import convertions
 
 import datetime
 import dataclasses
 
 import logging
 
 logger = logging.getLogger(__name__)
@@ -12,21 +13,21 @@
 class Metric:
     subject_type_id: str
     name: str
     id: str
     external_id: str
     data_type: str
     type: str
-    mapping_level: str = dataclasses.field(default=None)
-    created_date: datetime.datetime = dataclasses.field(default=None)
-    updated_date: datetime.datetime = dataclasses.field(default=None)
+    created_date: datetime.datetime
+    visible: bool = dataclasses.field(default=True)
     discrete: bool = dataclasses.field(default=False)
-    unit: str = dataclasses.field(default_factory=str)
-    precision: str = dataclasses.field(default_factory=str)
-    visible: bool = dataclasses.field(default_factory=bool)
+    mapping_level: Optional[str] = dataclasses.field(default=None)
+    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
+    unit: Optional[str] = dataclasses.field(default=None)
+    precision: Optional[str] = dataclasses.field(default=None)
 
     def __post_init__(self):
         if self.created_date:
             self.created_date = convertions.convert_any_date_to_datetime(
                 self.created_date
             )
         if self.updated_date:
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/property_type.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/property_type.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 class PropertyType:
     name: str
     external_id: str
     id: str
     created_date: datetime.datetime
     data_type: str
     predefined_values: bool
-    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
     values: List[property_value.PropertyValue] = dataclasses.field(default_factory=list)
+    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
 
     def __post_init__(self):
         if self.created_date:
             self.created_date = convertions.convert_any_date_to_datetime(
                 self.created_date
             )
         if self.updated_date:
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/property_value.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/property_value.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/series.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/series.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-from typing import List
+from typing import List, TypedDict
 
 from blockbax_sdk import errors
+from ..types import IngestionId
 from . import measurement
 
 import dataclasses
 import datetime
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
+class IngestionRequest(TypedDict, total=False):
+    ingestionId: IngestionId
+    measurements: List[measurement.MeasurementRequest]
+
+
+class SeriesRequest(TypedDict, total=False):
+    series: List[IngestionRequest]
+
+
 @dataclasses.dataclass
 class Series:
     subject_id: str
     metric_id: str
-    measurements: List[measurement.Measurement]
+    measurements: List[measurement.Measurement] = dataclasses.field(
+        default_factory=list
+    )
 
     def __iter__(self):
         return iter(self.measurements)
 
     @classmethod
     def from_api_response(cls, api_response):
         # Because we are constructing a new list there is no need to copy
@@ -36,11 +48,12 @@
             measurements=measurements,
         )
 
     @property
     def latest_date(self) -> datetime.datetime:
         latest_date = 0
         for measurement in self.measurements:
-            latest_date = (
-                measurement.date if measurement.date > latest_date else latest_date
-            )
+            if measurement.date is not None:
+                latest_date = (
+                    measurement.date if measurement.date > latest_date else latest_date
+                )
         return datetime.datetime.fromtimestamp(latest_date / 1000.0)
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/subject.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 @dataclasses.dataclass
 class Subject:
     name: str
     id: str
     subject_type_id: str
     external_id: str
     created_date: datetime.datetime
-    updated_date: datetime.datetime = dataclasses.field(default=None)
-    parent_id: Optional[str] = dataclasses.field(default=None)
     ingestion_ids: List[dict] = dataclasses.field(default_factory=list)
     properties: Dict[str, property_value.PropertyValue] = dataclasses.field(
         default_factory=dict
     )
+    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
+    parent_id: Optional[str] = dataclasses.field(default=None)
 
     def __post_init__(self):
         if self.created_date:
             self.created_date = convertions.convert_any_date_to_datetime(
                 self.created_date
             )
         if self.updated_date:
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/models/subject_type.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/models/subject_type.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 
 @dataclasses.dataclass
 class SubjectType:
     name: str
     id: str
     created_date: datetime.datetime
-    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
-    parent_ids: Optional[List[str]] = dataclasses.field(default=None)
     primary_location: Optional[dict] = dataclasses.field(default_factory=dict)
     property_types: Optional[List[dict]] = dataclasses.field(default_factory=list)
+    updated_date: Optional[datetime.datetime] = dataclasses.field(default=None)
+    parent_ids: Optional[List[str]] = dataclasses.field(default=None)
 
     def __post_init__(self):
         if self.created_date:
             self.created_date = convertions.convert_any_date_to_datetime(
                 self.created_date
             )
         if self.updated_date:
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/types.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing_extensions import Annotated, NewType, TypeGuard
-from typing import Any, TypeVar, Union
+from typing_extensions import TypeAlias, Annotated, TypedDict
+from typing import List, Optional, TypeVar, Union
 import datetime
 import enum
 import uuid
 from numbers import Number
 from decimal import Decimal
 
 import logging
@@ -26,20 +26,19 @@
 SubjectId = Annotated[BlockbaxId, "Subject"]
 MetricId = Annotated[BlockbaxId, "Metric"]
 PropertyTypeId = Annotated[BlockbaxId, "PropertyType"]
 SubjectTypeId = Annotated[BlockbaxId, "SubjectType"]
 
 # External ID' s
 SubjectExternalId = Annotated[BlockbaxExternalId, "Subject"]
-MetricExternalID = Annotated[BlockbaxExternalId, "Metric"]
+MetricExternalId = Annotated[BlockbaxExternalId, "Metric"]
 PropertyTypeExternalId = Annotated[BlockbaxExternalId, "PropertyType"]
 
 # Other ID
 IngestionId = Annotated[BlockbaxType[str], "Ingestion"]
-
 # Measurement data types
 
 
 class BxType(str, enum.Enum):
     @classmethod
     def _missing_(cls, value: object):
         if isinstance(value, str):
@@ -90,11 +89,53 @@
         known_types.append(member)
         if member.name == str(value).upper():
             return member
     error_unknown_type = f"'{value}' is not a known data type, known data types: {', '.join(known_types)}"
     raise ValueError(error_unknown_type)
 
 
-if __name__ == "__main__":
-    location_data_type = MeasurementDataTypes("location")
-    print(location_data_type)
-    print(type(location_data_type))
+class LocationLike(TypedDict, total=False):
+    lat: AnyNumber
+    lon: AnyNumber
+    alt: Optional[AnyNumber]
+
+
+class Location(TypedDict, total=False):
+    lat: Decimal
+    lon: Decimal
+    alt: Optional[Decimal]
+
+
+class MapLayerLike(TypedDict):
+    imagePath: str
+    leftBottom: LocationLike
+    leftTop: LocationLike
+    rightBottom: LocationLike
+    rightTop: LocationLike
+
+
+class MapLayer(TypedDict):
+    imagePath: str
+    leftBottom: Location
+    leftTop: Location
+    rightBottom: Location
+    rightTop: Location
+
+
+class Image(TypedDict):
+    imagePath: str
+
+
+class Polygon(TypedDict):
+    outerRing: List[Location]
+
+
+class Area(TypedDict):
+    polygon: Polygon
+
+
+class PolygonLike(TypedDict):
+    outerRing: List[LocationLike]
+
+
+class AreaLike(TypedDict):
+    polygon: PolygonLike
```

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/util/convertions.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/util/convertions.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/util/deprecated.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `blockbax_sdk-0.0.8/src/blockbax_sdk/util/validation.py` & `blockbax_sdk-0.0.9/src/blockbax_sdk/util/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import decimal
-from typing import List
+from typing_extensions import TypeGuard
+from typing import Any, Mapping, List, Optional, cast, Type, TypeVar
 
 from . import convertions
 from blockbax_sdk import types
 
 import logging
 
 logger = logging.getLogger(__name__)
 
+T = TypeVar("T")
 
-def validate_dict(name, dict_to_check: dict, keys: list):
+
+def validate_dict(
+    type: Type[T], dict_to_check: Mapping[Any, Any], keys: list
+) -> TypeGuard[T]:
     if not isinstance(dict_to_check, dict):
-        raise ValueError(
-            f"'{name}' with value `{dict_to_check}` is not a dict"
-        )  # TODO: update error mesage
+        raise ValueError(f"Dictionary `{dict_to_check}` is not a dict")
+    missing_keys = []
     for key in keys:
-        missing_keys = []
         if key not in dict_to_check:
             missing_keys.append(key)
     if len(missing_keys) > 0:
         raise ValueError(
-            f"'{name}' dict: {dict_to_check} does not have keys: {missing_keys}"
+            f"Dictionary is not of type '{type.__name__}', received value: {dict_to_check} does not have keys: {missing_keys}"
         )
+    return True
 
 
-def check_date_and_convert_to_unix(d: types.AnyDate) -> int:
+def check_date_and_convert_to_unix(d: Optional[types.AnyDate]) -> Optional[int]:
     """checks if the given date can be converted to a datetime object and returns the unix timestamp"""
+    if d is None:
+        return d
     return convertions.convert_any_date_to_unix_millis(d)
 
 
 def check_text(v: str) -> str:
     """checks if value is instance of str, or Text type, if not raise error"""
     if not isinstance(v, str):
         value_not_text_error = f"Text value {v} is not a Text type"
@@ -78,72 +84,76 @@
         altitude = convertions.convert_number_to_decimal(altitude)
         return altitude
     except (decimal.InvalidOperation, ValueError) as e:
         altitude_convertion_error = f"Could not convert: {altitude}, cause: {e}"
         raise ValueError(altitude_convertion_error)
 
 
-def check_location_and_convert(location: dict) -> dict:
+def check_location_and_convert(location: types.LocationLike) -> types.Location:
     # check if lat and lon are numeric and if the l dict has lat and lon
-    validate_dict("location", location, ["lat", "lon"])
+    validate_dict(types.Location, location, ["lat", "lon"])
 
-    location["lat"] = check_latitude_and_convert_to_decimal(location["lat"])
-    location["lon"] = check_longitude_and_convert_to_decimal(location["lon"])
+    if "lat" in location and "lon" in location:
+        location["lat"] = check_latitude_and_convert_to_decimal(location["lat"])
+        location["lon"] = check_longitude_and_convert_to_decimal(location["lon"])
     if "alt" in location:
         # altitude is optional
-        location["alt"] = check_altitude_and_convert_to_decimal(location["alt"])
-    return location
+        alt = location.get("alt")
+        if alt is not None:
+            location["alt"] = check_altitude_and_convert_to_decimal(alt)
+    return cast(types.Location, location)
 
 
-def check_map_layer_and_convert(map_layer: dict) -> dict:
+def check_map_layer_and_convert(map_layer: types.MapLayerLike) -> types.MapLayer:
     validate_dict(
-        "map_layer",
+        types.MapLayer,
         map_layer,
         ["imagePath", "leftBottom", "leftTop", "rightBottom", "rightTop"],
     )
 
     if not isinstance(map_layer["imagePath"], str):
         raise ValueError("'imagePath' is not a 'str'")
 
-    map_layer["leftBottom"] = check_location_and_convert(map_layer["leftBottom"])
-    map_layer["leftTop"] = check_location_and_convert(map_layer["leftTop"])
-    map_layer["rightBottom"] = check_location_and_convert(map_layer["rightBottom"])
-    map_layer["rightTop"] = check_location_and_convert(map_layer["rightTop"])
+    return {
+        "imagePath": map_layer["imagePath"],
+        "leftBottom": check_location_and_convert(map_layer["leftBottom"]),
+        "leftTop": check_location_and_convert(map_layer["leftTop"]),
+        "rightBottom": check_location_and_convert(map_layer["rightBottom"]),
+        "rightTop": check_location_and_convert(map_layer["rightTop"]),
+    }
 
-    return map_layer
 
-
-def check_image(image: dict):
-    validate_dict("image", image, ["imagePath"])
+def check_image(image: types.Image) -> types.Image:
+    validate_dict(types.Image, image, ["imagePath"])
 
     if not isinstance(image["imagePath"], str):
         raise ValueError("'imagePath' is not a 'str'")
 
     return image
 
 
 def list_contains_single_value(l: list) -> bool:
     summation = sum([value is not None for value in l])
     if summation > 1 or summation < 1:
         return False
     return True
 
 
-def check_and_convert_outer_ring(outer_ring: List[dict]):
-    new_outer_ring = []
-    for location in outer_ring:
-        new_outer_ring.append(check_location_and_convert(location))
-    return new_outer_ring
-
+def check_and_convert_outer_ring(
+    outer_ring: List[types.LocationLike],
+) -> List[types.Location]:
+    return [check_location_and_convert(location) for location in outer_ring]
 
-def check_and_convert_polygon(polygon: dict):
-    validate_dict("polygon", polygon, ["outerRing"])
 
-    polygon["outerRing"] = check_and_convert_outer_ring(polygon["outerRing"])
-    return polygon
+def check_and_convert_polygon(polygon: types.PolygonLike) -> types.Polygon:
+    validate_dict(types.Polygon, polygon, ["outerRing"])
 
+    return {
+        "outerRing": check_and_convert_outer_ring(polygon["outerRing"]),
+    }
 
-def check_area_and_convert(area: dict) -> dict:
-    validate_dict("area", area, ["polygon"])
 
-    area["polygon"] = check_and_convert_polygon(area["polygon"])
-    return area
+def check_area_and_convert(area: types.AreaLike) -> types.Area:
+    validate_dict(types.Area, area, ["polygon"])
+    return {
+        "polygon": check_and_convert_polygon(area["polygon"]),
+    }
```

### Comparing `blockbax_sdk-0.0.8/PKG-INFO` & `blockbax_sdk-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockbax-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Blockbax Python SDK
 Home-page: https://blockbax.com/docs/integrations/python-sdk/
 License: MIT
 Keywords: Blockbax,Data,Sensor,IoT
 Author: Blockbax
 Author-email: development@blockbax.com
 Maintainer: Blockbax
@@ -14,15 +14,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: httpx (>=0.23.3)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: pytz (>=2022.7.1)
 Requires-Dist: tenacity (>=8.1.0)
 Requires-Dist: typing-extensions (>=4.4.0)
 Project-URL: Documentation, https://blockbax.com/docs/python-sdk/
 Description-Content-Type: text/markdown
```

