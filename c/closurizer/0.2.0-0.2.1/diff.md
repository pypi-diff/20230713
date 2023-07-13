# Comparing `tmp/closurizer-0.2.0.tar.gz` & `tmp/closurizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closurizer-0.2.0.tar", max compression
+gzip compressed data, was "closurizer-0.2.1.tar", max compression
```

## Comparing `closurizer-0.2.0.tar` & `closurizer-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      641 2023-07-07 17:47:26.790480 closurizer-0.2.0/closurizer/cli.py
--rw-r--r--   0        0        0     4384 2023-07-07 17:47:26.790480 closurizer-0.2.0/closurizer/closurizer.py
--rw-r--r--   0        0        0      463 2023-07-07 17:47:26.790480 closurizer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      641 2023-07-13 00:15:40.582102 closurizer-0.2.1/closurizer/cli.py
+-rw-r--r--   0        0        0     4352 2023-07-13 00:15:40.582102 closurizer-0.2.1/closurizer/closurizer.py
+-rw-r--r--   0        0        0      463 2023-07-13 00:15:40.582102 closurizer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 closurizer-0.2.1/PKG-INFO
```

### Comparing `closurizer-0.2.0/closurizer/cli.py` & `closurizer-0.2.1/closurizer/cli.py`

 * *Files identical despite different names*

### Comparing `closurizer-0.2.0/closurizer/closurizer.py` & `closurizer-0.2.1/closurizer/closurizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,23 @@
         return 0
     else:
         return len(value.split("|"))
 
 def _length_of_field_values(rec, fields):
     value = 0
     for field in fields:
-        if field in rec and (field_value := rec[field]) is not None:
+        if (field_value := rec[field]) is not None:
             value += _length(field_value)
     return value
 
 def add_closure(kg_archive: str,
                 closure_file: str,
                 output_file: str,
                 fields: List[str] = ['subject', 'object'],
-                evidence_fields: List[str] = ['has_evidence', 'publications', 'primary_knowledge_source', 'provided_by']
+                evidence_fields: List[str] = ['has_evidence', 'publications', 'primary_knowledge_source']
                 ):
     print("Generating closure KG...")
     print(f"kg_archive: {kg_archive}")
     print(f"closure_file: {closure_file}")
 
     if fields is None or len(fields) == 0:
         fields = ['subject', 'object']
```

### Comparing `closurizer-0.2.0/PKG-INFO` & `closurizer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: closurizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Add closure expansion fields to kgx files following the Golr pattern
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

