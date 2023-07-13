# Comparing `tmp/yotpy-0.0.87.tar.gz` & `tmp/yotpy-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.87.tar", last modified: Mon Jun  5 17:54:25 2023, max compression
+gzip compressed data, was "yotpy-0.0.88.tar", last modified: Thu Jul 13 05:57:28 2023, max compression
```

## Comparing `yotpy-0.0.87.tar` & `yotpy-0.0.88.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.87/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.87/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.87/LICENSE
--rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.87/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.87/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.87/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.87/docs/yotpy.html
--rw-r--r--   0        0        0      847 2023-06-05 17:53:47.739564 yotpy-0.0.87/pyproject.toml
--rw-r--r--   0        0        0      318 2023-06-05 17:53:59.854921 yotpy-0.0.87/yotpy/__init__.py
--rw-r--r--   0        0        0    33804 2023-05-30 01:05:45.086759 yotpy-0.0.87/yotpy/core.py
--rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.87/yotpy/exceptions.py
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yotpy-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.88/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.88/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.88/LICENSE
+-rw-r--r--   0        0        0      378 2023-04-20 14:56:17.136904 yotpy-0.0.88/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.88/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.88/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.88/docs/yotpy.html
+-rw-r--r--   0        0        0      847 2023-06-05 17:53:47.739564 yotpy-0.0.88/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-07-13 05:56:36.958537 yotpy-0.0.88/yotpy/__init__.py
+-rw-r--r--   0        0        0    34571 2023-07-13 05:55:39.817008 yotpy-0.0.88/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.88/yotpy/exceptions.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 yotpy-0.0.88/PKG-INFO
```

### Comparing `yotpy-0.0.87/.github/workflows/static.yml` & `yotpy-0.0.88/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/LICENSE` & `yotpy-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/docs/search.js` & `yotpy-0.0.88/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/docs/yotpy.html` & `yotpy-0.0.88/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/pyproject.toml` & `yotpy-0.0.88/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/yotpy/core.py` & `yotpy-0.0.88/yotpy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         This method recursively traverses a nested JSON object and yields dictionaries containing the full key
         directory (as tuples) and their associated values. It handles dictionaries and lists within the JSON object.
 
         Example:
             Input JSON:
             ```python
             json = \\
-            { "a": 
+            { "a":
                 { "b":
                     [ { "c": "d" }, { "e": [1,2,3] } ]
                 },
               "x": { "y": "z" }
             }
             # Streaming key directories and values:
             >>> print(list(JSONTransformer.stream_json_data(json, tuple())))
@@ -119,15 +119,15 @@
         This method takes a nested JSON object and converts it into a dictionary with
         keys that represent the nested structure using a specified separator. Optionally,
         you can provide a list of keys to exclude or include in the resulting dictionary.
 
         Example:
             Input JSON:
             ```python
-            json = { "a": 
+            json = { "a":
                 { "b":
                     [ { "c": "d" }, { "e": [1,2,3] } ]
                 },
                 "x": { "y": "z" }
             }
             # Flattening with a "." separator:
             >>> print(JSONTransformer.flatten(json, "."))
@@ -169,15 +169,15 @@
 
     @staticmethod
     def flatten_list(json_list: list[dict], sep: str, exclude: list[str] = [], include: list[str] = []) -> list[dict[str, any]]:
         """
         Flattens a list of JSON objects into a list of dictionaries with flattened keys.
 
         This method takes a list of nested JSON objects and converts each JSON object into a
-        dictionary with keys representing the nested structure using a specified separator. 
+        dictionary with keys representing the nested structure using a specified separator.
         Optionally, you can provide a list of keys to exclude or include in the resulting dictionaries.
 
         Example:
             Input JSON list:
             ```python
             [
                 {
@@ -242,26 +242,27 @@
         """
         schema = list(iterator.schema)
         headers = {field.name for field in schema if (
             include and field.name in include) or (exclude and field.name not in exclude) or (not include and not exclude)}
 
         rows = []
         for row in iterator:
-            row = {field.name : row[field.name] for field in schema if field.name in headers}
+            row = {field.name: row[field.name]
+                   for field in schema if field.name in headers}
             rows.append(row)
-        
+
         return headers, rows
 
     @staticmethod
     def to_rows(json_list: list[dict], sep: str, exclude: list[str] = [], include: list[str] = []) -> tuple[list, set]:
         """
         Flatten a list of JSON objects into a list of rows and a set of headers.
 
         This method takes a list of nested JSON objects and converts each JSON object into a
-        dictionary with keys representing the nested structure using a specified separator. 
+        dictionary with keys representing the nested structure using a specified separator.
         It then creates a list of rows, where each row contains the values from the flattened
         dictionaries, and a set of headers representing the unique keys of the flattened dictionaries.
 
         Args:
             json_list (list[dict]): The list of JSON objects to flatten.
             sep (str): The separator to use for joining nested keys.
             exclude (list[str]): If specified, exclude keys that match the specified keys and include all others.
@@ -301,15 +302,16 @@
 
         Returns:
             StringIO: A CSV formatted StringIO object.
         """
         # Create a StringIO object to write the CSV data to.
         csv_stringio = StringIO()
         # Create a csv writer and write the rows to the StringIO object.
-        writer = DictWriter(csv_stringio, fieldnames=headers, delimiter=delimiter)
+        writer = DictWriter(
+            csv_stringio, fieldnames=headers, delimiter=delimiter)
         writer.writeheader()
         writer.writerows(rows)
 
         # Reset the StringIO object's position to the beginning
         csv_stringio.seek(0)
 
         return csv_stringio
@@ -329,59 +331,75 @@
             delimiter (str, optional): The delimiter to use for the CSV data. Defaults to ','.
 
         Returns:
             BytesIO: A CSV formatted BytesIO object.
         """
         # Create a BytesIO object to write the CSV data to.
         csv_bytesio = BytesIO()
-        
+
         # Wrap the BytesIO object with a TextIOWrapper using utf-8-sig encoding.
         csv_textio = TextIOWrapper(csv_bytesio, encoding='utf-8-sig')
 
         # Create a csv writer and write the rows to the wrapped BytesIO object.
-        writer = DictWriter(csv_textio, fieldnames=headers, delimiter=delimiter)
+        writer = DictWriter(csv_textio, fieldnames=headers,
+                            delimiter=delimiter)
         writer.writeheader()
         writer.writerows(rows)
 
         # Flush the TextIOWrapper to ensure all data is written to the underlying BytesIO object
         csv_textio.flush()
 
         csv_bytesio = csv_textio.detach()
 
         # Reset the BytesIO object's position to the beginning
         csv_bytesio.seek(0)
 
         return csv_bytesio
 
     @staticmethod
-    def to_xlsx_bytesio(headers: set, rows: list[dict]) -> BytesIO:
+    def to_xlsx_bytesio(headers: set, rows: list[dict], helper: bool = False) -> BytesIO:
         """
         Convert a list of rows into a Excel formatted BytesIO object.
 
         This method takes a list of rows (dictionaries) and a set of headers, and writes them into
         an Excel formatted BytesIO object. It can be used to create an Excel file-like object without
         creating an actual file on the filesystem.
 
         Args:
             headers (set): A set of headers to use for the Excel data.
             rows (list[dict]): A list of rows to convert into an Excel formatted BytesIO object.
+            helper (bool, optional): If True, enables automatic parsing and filling of unformatted data. Defaults to False.
 
         Returns:
             BytesIO: An Excel formatted BytesIO object.
         """
+
+        # Helper function used to parse a usable value when a value error is throw.
+        def value_parser(value, header):
+            if isinstance(value, list | set):
+                return value.pop() if len(value) else ""
+            elif isinstance(value, tuple):
+                return value[0] if len(value) else ""
+            elif isinstance(value, dict):
+                return value.get(header, "")
+
         # Create a Workbook object
         wb = Workbook()
         ws = wb.active
 
         # Write headers
         ws.append(list(headers))
 
         # Write rows
         for row in rows:
-            ws.append([row[h] for h in headers])
+            for header in headers:
+                try:
+                    ws.append(row[header])
+                except ValueError:
+                    ws.append(value_parser(row[header], header))
 
         # Save workbook to a BytesIO object
         xlsx_bytesio = BytesIO()
         wb.save(xlsx_bytesio)
 
         # Reset the BytesIO object's position to the beginning
         xlsx_bytesio.seek(0)
```

### Comparing `yotpy-0.0.87/yotpy/exceptions.py` & `yotpy-0.0.88/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.87/PKG-INFO` & `yotpy-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.87
+Version: 0.0.88
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

