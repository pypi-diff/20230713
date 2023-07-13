# Comparing `tmp/reasoner_validator-3.7.1.tar.gz` & `tmp/reasoner_validator-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.1.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.2.tar", max compression
```

## Comparing `reasoner_validator-3.7.1.tar` & `reasoner_validator-3.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1153 2023-07-12 20:45:57.725284 reasoner_validator-3.7.1/LICENSE
--rw-r--r--   0        0        0    12703 2023-07-12 20:45:57.725284 reasoner_validator-3.7.1/README.md
--rw-r--r--   0        0        0      131 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/conf.py
--rw-r--r--   0        0        0    19869 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36258 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2177 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/pyproject.toml
--rw-r--r--   0        0        0    38452 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    75056 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39514 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/message.py
--rw-r--r--   0        0        0    29459 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11643 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    12532 2023-07-12 20:45:57.729285 reasoner_validator-3.7.1/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      774 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/conftest.py
--rw-r--r--   0        0        0   117951 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    40085 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26808 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_validate.py
--rw-r--r--   0        0        0    21576 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-12 20:45:57.733285 reasoner_validator-3.7.1/tests/test_workflows.py
--rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/LICENSE
+-rw-r--r--   0        0        0    12703 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/README.md
+-rw-r--r--   0        0        0      131 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/conf.py
+-rw-r--r--   0        0        0    19869 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36258 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2177 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/pyproject.toml
+-rw-r--r--   0        0        0    38452 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    75092 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39514 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/message.py
+-rw-r--r--   0        0        0    29568 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11643 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    12532 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      774 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/conftest.py
+-rw-r--r--   0        0        0   117951 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40085 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26808 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_validate.py
+-rw-r--r--   0        0        0    21570 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_workflows.py
+-rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.2/PKG-INFO
```

### Comparing `reasoner_validator-3.7.1/LICENSE` & `reasoner_validator-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/README.md` & `reasoner_validator-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/docs/Makefile` & `reasoner_validator-3.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/docs/conf.py` & `reasoner_validator-3.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/docs/index.rst` & `reasoner_validator-3.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/docs/make.bat` & `reasoner_validator-3.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.2/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/pyproject.toml` & `reasoner_validator-3.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.1"
+version = "3.7.2"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.7.1/reasoner_validator/__init__.py` & `reasoner_validator-3.7.2/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.2/reasoner_validator/biolink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1241,15 +1241,15 @@
                 source_trail=source_trail,
                 identifier=object_id,
                 edge_id=edge_id
             )
 
     # TODO: 11-July-2023: Certain specific 'abstract' or 'mixin' categories used in Knowledge Graphs
     #                     are being validated for now as 'warnings', for short term validation purposes
-    CATEGORY_INCLUSIONS = ["biolink:BiologicalEntity"]
+    CATEGORY_INCLUSIONS = ["biolink:BiologicalEntity", "biolink:InformationContentEntity"]
 
     def validate_category(
             self,
             context: str,
             node_id: Optional[str],
             category: Optional[str]
     ) -> ClassDefinition:
```

### Comparing `reasoner_validator-3.7.1/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.2/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/message.py` & `reasoner_validator-3.7.2/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/report.py` & `reasoner_validator-3.7.2/reasoner_validator/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Error and Warning Reporting Module"""
 from typing import Optional, Dict, List
 from sys import stdout
+from importlib import metadata
 from io import StringIO
 import copy
 
 from json import dumps, JSONEncoder
 
 from reasoner_validator.message import (
     MESSAGE_CATALOG,
@@ -467,18 +468,18 @@
                 print(f"\n\033[4m{title}\033[0m", file=file)
                 print(file=file)
             else:
                 # compact also ignores underlining
                 print(title, file=file)
 
         print(
-            "Validation against TRAPI " +
-            f"'{str(self.trapi_version if self.trapi_version is not None else 'Default')}' version " +
-            "and Biolink Model " +
-            f"'{str(self.biolink_version if self.biolink_version is not None else 'Default')}' version.",
+            f"Reasoner Validator version '{metadata.version('reasoner-validator')}' validating against "
+            f"TRAPI schema version '{str(self.trapi_version if self.trapi_version is not None else 'Default')}' " +
+            "and Biolink Model version " +
+            f"'{str(self.biolink_version if self.biolink_version is not None else 'Default')}'.\n",
             file=file
         )
 
         if self.has_messages():
 
             # self.messages is a MESSAGE_CATALOG where MESSAGE_CATALOG is Dict[<message type>, MESSAGE_PARTITION]
             # <message type> is the top level partition of messages into 'critical', 'error', 'warning' or 'info'
```

### Comparing `reasoner_validator-3.7.1/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.2/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.2/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.2/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.2/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/reasoner_validator/versioning.py` & `reasoner_validator-3.7.2/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/__init__.py` & `reasoner_validator-3.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.2/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_response_validator.py` & `reasoner_validator-3.7.2/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_semver.py` & `reasoner_validator-3.7.2/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.2/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_validate.py` & `reasoner_validator-3.7.2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/tests/test_validation_report.py` & `reasoner_validator-3.7.2/tests/test_validation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         "ValidatorReporter.dump() resetting the title to a user string\n" +
         "and compressed using 'id_rows=1', 'msg_rows=1', 'compress=True':\n",
         file=stderr
     )
     reporter1.dump(title="My KP Validation Report", id_rows=1, msg_rows=1, compact_format=True, file=stderr)
 
     validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
-    assert validation_report.startswith("Validation against TRAPI")
+    assert validation_report.startswith("Reasoner Validator")
 
 
 def test_validator_method():
 
     reporter = ValidationReporter(
         prefix="Test Validator Method",
         trapi_version=TEST_TRAPI_VERSION,
```

### Comparing `reasoner_validator-3.7.1/tests/test_workflows.py` & `reasoner_validator-3.7.2/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.1/PKG-INFO` & `reasoner_validator-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.1
+Version: 3.7.2
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

