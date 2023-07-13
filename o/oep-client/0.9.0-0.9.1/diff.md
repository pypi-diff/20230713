# Comparing `tmp/oep-client-0.9.0.tar.gz` & `tmp/oep-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\oep-client-0.9.0.tar", last modified: Wed Aug 25 14:13:01 2021, max compression
+gzip compressed data, was "dist\oep-client-0.9.1.tar", last modified: Tue Sep 28 06:20:36 2021, max compression
```

## Comparing `oep-client-0.9.0.tar` & `oep-client-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-08-25 14:13:01.000000 oep-client-0.9.0/
--rw-rw-rw-   0        0        0    35823 2020-03-30 06:29:13.000000 oep-client-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     7982 2021-08-25 14:13:01.000000 oep-client-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     7561 2021-06-15 10:03:57.000000 oep-client-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2021-08-25 14:13:01.000000 oep-client-0.9.0/oep_client/
--rw-rw-rw-   0        0        0      439 2021-08-25 14:12:24.000000 oep-client-0.9.0/oep_client/__init__.py
--rw-rw-rw-   0        0        0     7618 2021-08-25 14:12:24.000000 oep-client-0.9.0/oep_client/cli.py
--rw-rw-rw-   0        0        0    20234 2021-08-25 14:12:13.000000 oep-client-0.9.0/oep_client/oep_client.py
--rw-rw-rw-   0        0        0     2098 2021-08-25 14:12:12.000000 oep-client-0.9.0/oep_client/test.py
-drwxrwxrwx   0        0        0        0 2021-08-25 14:13:01.000000 oep-client-0.9.0/oep_client.egg-info/
--rw-rw-rw-   0        0        0     7982 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-08-25 14:12:59.000000 oep-client-0.9.0/oep_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-25 14:13:01.000000 oep-client-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      759 2021-08-25 14:12:24.000000 oep-client-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-28 06:20:36.000000 oep-client-0.9.1/
+-rw-rw-rw-   0        0        0    35823 2020-03-30 06:29:13.000000 oep-client-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     7982 2021-09-28 06:20:36.000000 oep-client-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7561 2021-06-15 10:03:57.000000 oep-client-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2021-09-28 06:20:36.000000 oep-client-0.9.1/oep_client/
+-rw-rw-rw-   0        0        0      439 2021-09-28 06:20:14.000000 oep-client-0.9.1/oep_client/__init__.py
+-rw-rw-rw-   0        0        0     7618 2021-09-28 06:20:14.000000 oep-client-0.9.1/oep_client/cli.py
+-rw-rw-rw-   0        0        0    23387 2021-09-28 06:16:56.000000 oep-client-0.9.1/oep_client/oep_client.py
+-rw-rw-rw-   0        0        0     2098 2021-08-25 14:12:12.000000 oep-client-0.9.1/oep_client/test.py
+drwxrwxrwx   0        0        0        0 2021-09-28 06:20:36.000000 oep-client-0.9.1/oep_client.egg-info/
+-rw-rw-rw-   0        0        0     7982 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2021-09-28 06:20:33.000000 oep-client-0.9.1/oep_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-09-28 06:20:36.000000 oep-client-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      759 2021-09-28 06:20:14.000000 oep-client-0.9.1/setup.py
```

### Comparing `oep-client-0.9.0/LICENSE` & `oep-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oep-client-0.9.0/PKG-INFO` & `oep-client-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oep-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: client side tool for openenergy platform
 Home-page: https://github.com/wingechr/oep-client
 Author: Christian Winger
 Author-email: c.winger@oeko.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oep-client-0.9.0/README.md` & `oep-client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `oep-client-0.9.0/oep_client/cli.py` & `oep-client-0.9.1/oep_client/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Command line script for OepClient
 """
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 import sys
 import logging
 import json
 import re
 
 import click
```

### Comparing `oep-client-0.9.0/oep_client/oep_client.py` & `oep-client-0.9.1/oep_client/oep_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 import click
 import requests
 
 
 DEFAULT_HOST = "https://openenergy-platform.org"
 DEFAULT_API_VERSION = "v0"
 DEFAULT_SCHEMA = "model_draft"
-DEFAULT_BATCH_SIZE = None
-DEFAULT_INSERT_RETRIES = 0
+DEFAULT_BATCH_SIZE = 5000
+DEFAULT_INSERT_RETRIES = 10
 
 
 class OepApiException(Exception):
     pass
 
 
 class OepServerSideException(OepApiException):
@@ -257,29 +257,26 @@
                 defaults to self.default_schema which is usually "model_draft"
             batch_size(int, optional): defaults to client's default batch size
             method(list, optional):
                 * 'api': sent records via regular API
                 * 'advanced' (default): sent records via advanced API
         """
 
-        table_def = self._get_table_definition(table, schema=schema)
-        column_names = [
-            c["name"]
-            for c in sorted(table_def["columns"], key=lambda c: c["ordinal_position"])
-        ]
+        table_def = self.get_table_definition(table, schema=schema)
+        column_names = [c["name"] for c in table_def["columns"]]
         used_column_names = set()
         for row in data:
             used_column_names = used_column_names | set(row.keys())
         unknown_column_names = used_column_names - set(column_names)
         if unknown_column_names:
             raise OepClientSideException(
                 "Columns not in table: %s", unknown_column_names
             )
 
-        batch_size = (batch_size or self.batch_size) or 1
+        batch_size = batch_size or self.batch_size
         n_batches = math.ceil(len(data) / batch_size)
         data_batches = [
             data[i * batch_size : (i + 1) * batch_size] for i in range(n_batches)
         ]
 
         n_items = 0
         with click.progressbar(data_batches) as data_parts:
@@ -332,50 +329,129 @@
             return {}
 
         url = self._get_table_url(table=table, schema=schema) + "rows/new"
         res = self._request("POST", url, 201, {"query": data})
         return res
 
     @check_exception("not found", OepTableNotFoundException)
-    def _get_table_definition(self, table, schema=None):
+    def get_table_definition(self, table, schema=None):
         """Returns table info
 
         Args:
             table(str): table name. Must be valid postgres table name,
                 all lowercase, only letters, numbers and underscore
 
             schema(str, optional): table schema name.
                 defaults to self.default_schema which is usually "model_draft"
         """
         url = self._get_table_url(table=table, schema=schema)
         res = self._request("GET", url, 200)
+        definition = {
+            "columns": [],
+            "constraints": [],
+        }
+
+        # res["columns"] is dict
+        # first: add constrains to field definitions / constraints
+        for const in res["constraints"].values():
+            const_type = const["constraint_type"]
+            const_def = const["definition"]
+            if const_type == "PRIMARY KEY":
+                args = re.match(
+                    r"^PRIMARY KEY \((?P<field>[^)]+)\)$", const_def
+                ).groupdict()
+                # NOTE currently only single field PK allowed
+                res["columns"][args["field"]]["primary_key"] = True
+            elif const_type == "FOREIGN KEY":
+                args = re.match(
+                    r"^FOREIGN KEY \((?P<field>[^)]+)\) REFERENCES (?P<ref_schema>[^.]+)\.(?P<ref_table>[^()]+)\((?P<ref_field>[^)]+)\)$",
+                    const_def,
+                ).groupdict()
+                # NOTE currently only single field PK allowed
+                res["columns"][args["field"]]["foreign_key"] = [
+                    {
+                        "schema": args["ref_schema"],
+                        "table": args["ref_table"],
+                        "column": args["ref_field"],
+                    }
+                ]
+            elif const_type == "UNIQUE":
+                args = re.match(
+                    r"^UNIQUE \((?P<fields>[^)]+)\)$", const_def
+                ).groupdict()
+                columns = [f.strip() for f in args["fields"].split(",")]
+                definition["constraints"].append(
+                    {"constraint_type": "UNIQUE", "columns": columns}
+                )
+
+        def get_datatype(coldef):
+            dt = coldef["data_type"].upper()
+            if dt == "CHARACTER":
+                dt = "CHAR(%d)" % coldef["character_maximum_length"]
+            elif dt == "CHARACTER VARYING":
+                dt = "VARCHAR(%d)" % coldef["character_maximum_length"]
+            elif dt == "DOUBLE PRECISION":
+                dt = "FLOAT"
+
+            if (coldef["column_default"] or "").startswith("nextval"):
+                if not "INT" in dt:
+                    raise NotImplementedError(dt)
+                else:
+                    dt = dt.replace("INT", "SERIAL")
+
+            return dt
+
         # fix columns: list instead of dict
-        for name, col in res["columns"].items():
-            col["name"] = name
-        res["columns"] = sorted(
-            res["columns"].values(), key=lambda c: c["ordinal_position"]
-        )
-        return res
+        for name, coldef in sorted(
+            res["columns"].items(), key=lambda c: c[1]["ordinal_position"]
+        ):
+            col = {
+                "name": name,
+                "data_type": get_datatype(coldef),
+                "is_nullable": coldef["is_nullable"],
+            }
+            if coldef.get("primary_key", False):
+                col["primary_key"] = True
+            if "foreign_key" in coldef:
+                col["foreign_key"] = coldef["foreign_key"]
+            definition["columns"].append(col)
+
+        return definition
 
     def table_exists(self, table, schema=None):
         """True or False
 
         Args:
             table(str): table name. Must be valid postgres table name,
                 all lowercase, only letters, numbers and underscore
 
             schema(str, optional): table schema name.
                 defaults to self.default_schema which is usually "model_draft"
         """
+
         try:
-            self._get_table_definition(table, schema)
-            return True
+            return self._table_exists(table, schema)
         except OepTableNotFoundException:
             return False
 
+    @check_exception("not found", OepTableNotFoundException)
+    def _table_exists(self, table, schema=None):
+        """True or False
+
+        Args:
+            table(str): table name. Must be valid postgres table name,
+                all lowercase, only letters, numbers and underscore
+
+            schema(str, optional): table schema name.
+                defaults to self.default_schema which is usually "model_draft"
+        """
+        url = self._get_table_url(table=table, schema=schema)
+        self._request("GET", url, 200)
+        return True
+
     def get_metadata(self, table, schema=None):
         """Returns metadata json
 
         Args:
             table(str): table name. Must be valid postgres table name,
                 all lowercase, only letters, numbers and underscore
 
@@ -496,22 +572,22 @@
             logging.debug("Closed cursor: %s", self.cursor_id)
             self.cursor_id = None
         if self.connection_id:
             self._command("connection/close")
             logging.debug("Closed connection: %s", self.connection_id)
             self.connection_id = None
 
-    def insert_into_table(self, table, data, schema):
+    def insert_into_table(self, table, data, schema=None):
         """Insert records into table.
 
         Args:
             table(str): table name. Must be valid postgres table name,
                 all lowercase, only letters, numbers and underscore
             data(list): list of records(dict: column_name -> value)
-            schema(str): table schema name.
+            schema(str, optional): table schema name.
                 defaults to self.default_schema which is usually "model_draft"
         """
 
         if not isinstance(data, (list, tuple)) or (
             data and not isinstance(data[0], dict)
         ):
             raise OepClientSideException(
```

### Comparing `oep-client-0.9.0/oep_client/test.py` & `oep-client-0.9.1/oep_client/test.py`

 * *Files identical despite different names*

### Comparing `oep-client-0.9.0/oep_client.egg-info/PKG-INFO` & `oep-client-0.9.1/oep_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oep-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: client side tool for openenergy platform
 Home-page: https://github.com/wingechr/oep-client
 Author: Christian Winger
 Author-email: c.winger@oeko.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oep-client-0.9.0/setup.py` & `oep-client-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="oep-client",
-    version="0.9.0",
+    version="0.9.1",
     description="client side tool for openenergy platform",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=["oep_client"],
     author="Christian Winger",
     author_email="c.winger@oeko.de",
     url="https://github.com/wingechr/oep-client",
```

