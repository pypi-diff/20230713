# Comparing `tmp/satori_playbook_validator-3.1.1.tar.gz` & `tmp/satori_playbook_validator-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-3.1.1.tar", last modified: Thu Jun 29 16:49:36 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.1.2.tar", last modified: Thu Jul 13 21:03:23 2023, max compression
```

## Comparing `satori_playbook_validator-3.1.1.tar` & `satori_playbook_validator-3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/README.md
--rw-r--r--   0        0        0      474 2023-06-29 16:49:36.273807 satori_playbook_validator-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      301 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5920 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      298 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1906 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2361 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      100 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/src/satorici/validator/warnings.py
--rw-r--r--   0        0        0     2659 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-29 16:49:19.465604 satori_playbook_validator-3.1.1/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/README.md
+-rw-r--r--   0        0        0      518 2023-07-13 21:03:23.111551 satori_playbook_validator-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     6168 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      298 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1906 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     2659 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.2/PKG-INFO
```

### Comparing `satori_playbook_validator-3.1.1/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.1.2/src/satorici/validator/_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import re
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from urllib.parse import urlsplit
 
+from aws_cron_expression_validator.validator import AWSCronExpressionValidator
 from fastjsonschema import JsonSchemaValueException, compile
 
 from .exceptions import (
     NoExecutionsError,
     PlaybookValidationError,
     PlaybookVariableError,
 )
@@ -89,14 +90,19 @@
     return _is(validate_test, test)
 
 
 def validate_settings(settings: dict):
     _validate(settings_schema, settings)
 
     if "cron" in settings or "rate" in settings:
+        try:
+            AWSCronExpressionValidator.validate(settings["cron"])
+        except Exception:
+            PlaybookValidationError("Invalid cron expression")
+
         if not any(k.startswith("log") for k in settings):
             warnings.warn(NoLogMonitorWarning("Monitor without notifications."))
 
     if "timeout" in settings and "commandTimeout" in settings:
         if settings["timeout"] < settings["commandTimeout"]:
             raise PlaybookValidationError("timeout must be greater than commandTimeout")
```

### Comparing `satori_playbook_validator-3.1.1/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.1/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.1/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.1/tests/test_playbook_validator.py` & `satori_playbook_validator-3.1.2/tests/test_playbook_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.1/tests/test_reference_finder.py` & `satori_playbook_validator-3.1.2/tests/test_reference_finder.py`

 * *Files identical despite different names*

