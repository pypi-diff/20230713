# Comparing `tmp/meltanolabs_target_snowflake-0.4.1.tar.gz` & `tmp/meltanolabs_target_snowflake-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.4.1.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.4.2.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.4.1.tar` & `meltanolabs_target_snowflake-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3860 2023-07-12 16:00:16.032357 meltanolabs_target_snowflake-0.4.1/LICENSE
--rw-r--r--   0        0        0     5010 2023-07-12 16:00:16.032357 meltanolabs_target_snowflake-0.4.1/README.md
--rw-r--r--   0        0        0     1307 2023-07-12 16:00:40.672572 meltanolabs_target_snowflake-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       89 2023-07-12 16:00:40.672572 meltanolabs_target_snowflake-0.4.1/target_snowflake/__init__.py
--rw-r--r--   0        0        0    19306 2023-07-12 16:00:16.036357 meltanolabs_target_snowflake-0.4.1/target_snowflake/connector.py
--rw-r--r--   0        0        0     2651 2023-07-12 16:00:16.036357 meltanolabs_target_snowflake-0.4.1/target_snowflake/initializer.py
--rw-r--r--   0        0        0     8248 2023-07-12 16:00:16.036357 meltanolabs_target_snowflake-0.4.1/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-07-12 16:00:16.036357 meltanolabs_target_snowflake-0.4.1/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     3147 2023-07-12 16:00:16.036357 meltanolabs_target_snowflake-0.4.1/target_snowflake/target.py
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5010 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/README.md
+-rw-r--r--   0        0        0     1332 2023-07-13 16:55:52.014536 meltanolabs_target_snowflake-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-13 16:55:52.014536 meltanolabs_target_snowflake-0.4.2/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    19556 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/connector.py
+-rw-r--r--   0        0        0     2651 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/initializer.py
+-rw-r--r--   0        0        0     8248 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     3147 2023-07-13 16:55:25.970246 meltanolabs_target_snowflake-0.4.2/target_snowflake/target.py
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.4.2/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.4.1/LICENSE` & `meltanolabs_target_snowflake-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/README.md` & `meltanolabs_target_snowflake-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/pyproject.toml` & `meltanolabs_target_snowflake-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.4.1"
+version = "0.4.2"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
@@ -18,14 +18,15 @@
 requests = "^2.31.0"
 snowflake-sqlalchemy = "^1.4.7"
 singer-sdk = "0.30.0"
 cryptography = "^40.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
+pytest-xdist = ">=3.3.1"
 singer-sdk = { version="0.30.0", extras = ["testing"] }
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 
 [tool.ruff]
 ignore = [
```

### Comparing `meltanolabs_target_snowflake-0.4.1/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.4.2/target_snowflake/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from snowflake.sqlalchemy.base import SnowflakeIdentifierPreparer
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 from sqlalchemy.engine import Engine
 from sqlalchemy.sql import text
 
 from target_snowflake.snowflake_types import NUMBER, TIMESTAMP_NTZ, VARIANT
 
-
 SNOWFLAKE_MAX_STRING_LENGTH = 16777216
 
 class TypeMap:
     def __init__(self, operator, map_value, match_value=None):
         self.operator = operator
         self.map_value = map_value
         self.match_value = match_value
@@ -266,15 +265,15 @@
                 schema_name = schema_name.upper()
             return schema_name in schema_names
 
     # Custom SQL get methods
 
     def _get_put_statement(self, sync_id: str, file_uri: str) -> Tuple[text, dict]:
         """Get Snowflake PUT statement."""
-        return (text(f"put '{file_uri}' '@~/target-snowflake/{sync_id}'"), {})
+        return (text(f"put :file_uri '@~/target-snowflake/{sync_id}'"), {})
 
     def _get_column_selections(self, schema: dict, formatter: SnowflakeIdentifierPreparer) -> list:
         column_selections = []
         for property_name, property_def in schema["properties"].items():
             clean_property_name = formatter.format_collation(property_name)
             clean_alias = clean_property_name
             if '"' in clean_property_name:
@@ -368,15 +367,17 @@
             files: The files containing records to upload.
         """
         with self._connect() as conn:
             for file_uri in files:
                 put_statement, kwargs = self._get_put_statement(
                     sync_id=sync_id, file_uri=file_uri
                 )
-                conn.execute(put_statement, **kwargs)
+                # sqlalchemy.text stripped a slash, which caused windows to fail so we used bound parameters instead
+                # See https://github.com/MeltanoLabs/target-snowflake/issues/87 for more information about this error
+                conn.execute(put_statement, file_uri=file_uri, **kwargs)
 
     def create_file_format(self, file_format: str) -> None:
         """Create a file format in the schema.
 
         Args:
             file_format: The name of the file format.
         """
```

### Comparing `meltanolabs_target_snowflake-0.4.1/target_snowflake/initializer.py` & `meltanolabs_target_snowflake-0.4.2/target_snowflake/initializer.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.4.2/target_snowflake/sinks.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.4.2/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.4.2/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.4.1/PKG-INFO` & `meltanolabs_target_snowflake-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.4.1
+Version: 0.4.2
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

