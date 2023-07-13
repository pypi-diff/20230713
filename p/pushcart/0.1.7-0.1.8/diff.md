# Comparing `tmp/pushcart-0.1.7.tar.gz` & `tmp/pushcart-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-0.1.7.tar", max compression
+gzip compressed data, was "pushcart-0.1.8.tar", max compression
```

## Comparing `pushcart-0.1.7.tar` & `pushcart-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.7/LICENSE
--rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.7/pushcart/__init__.py
--rw-r--r--   0        0        0    13589 2023-07-13 19:37:18.998215 pushcart-0.1.7/pushcart/metadata.py
--rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.7/pushcart/utils.py
--rw-r--r--   0        0        0     2543 2023-07-13 19:41:53.261558 pushcart-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.8/LICENSE
+-rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.8/pushcart/__init__.py
+-rw-r--r--   0        0        0    13729 2023-07-13 21:16:30.451753 pushcart-0.1.8/pushcart/metadata.py
+-rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.8/pushcart/utils.py
+-rw-r--r--   0        0        0     2543 2023-07-13 21:18:31.048424 pushcart-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.8/PKG-INFO
```

### Comparing `pushcart-0.1.7/LICENSE` & `pushcart-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.7/pushcart/metadata.py` & `pushcart-0.1.8/pushcart/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,16 @@
 def _infer_timestamps(df: DataFrame, column_name: str) -> str:
     log.info(f"Attempting to infer timestamp format for {column_name} column.")
 
     pd_ts_format = None
 
     with contextlib.suppress(ParserError, AttributeError, TypeError):
         pd_ts_df = df.select(column_name).dropna().limit(1).toPandas()
-        pd_ts_list = pd_ts_df[column_name].to_numpy()
+        # Pandas keeps the last bit of the field path as column name
+        pd_ts_list = pd_ts_df[column_name.split(".")[-1]].to_numpy()
 
         pd_ts_format = _guess_datetime_format_for_array(pd_ts_list)
 
     if not pd_ts_format:
         log.warning(f"Could not infer timestamp format for {column_name} column.")
         return None
 
@@ -262,53 +263,51 @@
                 )
 
         return ""
 
     def _generate_field(self, field: T.StructField, parent: str = None) -> dict:
         name = field.name
         dtype = field.dataType
+        flat_parent = parent.replace(".", "_") if parent else None
         return {
-            "source_column_name": f"{parent}.{name}" if parent else name,
+            "source_column_name": f"{flat_parent}.{name}" if parent else name,
             "source_column_type": dtype.simpleString(),
-            "dest_column_name": f"{parent.replace('.', '_')}_{name}"
-            if parent
-            else name,
+            "dest_column_name": f"{flat_parent}_{name}" if parent else name,
             "dest_column_type": dtype.elementType.simpleString()
             if isinstance(dtype, T.ArrayType)
             else dtype.simpleString(),
-            "transform_function": f'F.explode("{name}")'
+            "transform_function": f'F.explode("{flat_parent}.{name}")'
             if isinstance(dtype, T.ArrayType)
-            else self._infer(name)
+            else self._infer(f"{parent}.{name}" if parent else name)
             if isinstance(dtype, T.StringType)
             else "",
             "default_value": "",
             "validation_rule": "",
             "validation_action": "",
         }
 
-    def _generate(self, schema: T.StructType, parent: None) -> list:
+    def _generate(self, schema: T.StructType, parent: str = None) -> list:
         fields = []
 
         for f in schema.fields:
-            # Drop technical fields
-            if f.name.startswith("_"):
-                continue
-
             dtype = f.dataType
 
             field_name = f"{parent + '.' if parent else ''}{f.name}"
 
             if isinstance(dtype, T.ArrayType) and isinstance(
-                f.dataType.elementType,
+                dtype.elementType,
                 T.StructType,
             ):
                 fields.append(self._generate_field(f, parent))
-                fields += self._generate(dtype.elementType, field_name)
+                fields += self._generate(
+                    dtype.elementType,
+                    parent=field_name,
+                )
             elif isinstance(dtype, T.StructType):
-                fields += self._generate(dtype, field_name)
+                fields += self._generate(dtype, parent=field_name)
             else:
                 fields.append(self._generate_field(f, parent))
 
         return fields
 
     def generate(self) -> pd.DataFrame:
         """Generate a Pandas DataFrame containing the metadata for the dataset being analyzed.
```

### Comparing `pushcart-0.1.7/pushcart/utils.py` & `pushcart-0.1.8/pushcart/utils.py`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.7/pyproject.toml` & `pushcart-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart"
-version = "0.1.7"
+version = "0.1.8"
 description = "Metadata transformations for Spark"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `pushcart-0.1.7/PKG-INFO` & `pushcart-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushcart
-Version: 0.1.7
+Version: 0.1.8
 Summary: Metadata transformations for Spark
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

