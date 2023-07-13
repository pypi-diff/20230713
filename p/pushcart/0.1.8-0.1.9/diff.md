# Comparing `tmp/pushcart-0.1.8.tar.gz` & `tmp/pushcart-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart-0.1.8.tar", max compression
+gzip compressed data, was "pushcart-0.1.9.tar", max compression
```

## Comparing `pushcart-0.1.8.tar` & `pushcart-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.8/LICENSE
--rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.8/pushcart/__init__.py
--rw-r--r--   0        0        0    13729 2023-07-13 21:16:30.451753 pushcart-0.1.8/pushcart/metadata.py
--rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.8/pushcart/utils.py
--rw-r--r--   0        0        0     2543 2023-07-13 21:18:31.048424 pushcart-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-08 07:35:44.283369 pushcart-0.1.9/LICENSE
+-rw-r--r--   0        0        0       80 2023-07-08 07:35:44.303369 pushcart-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 07:34:25.976683 pushcart-0.1.9/pushcart/__init__.py
+-rw-r--r--   0        0        0    14232 2023-07-13 21:38:54.698467 pushcart-0.1.9/pushcart/metadata.py
+-rw-r--r--   0        0        0     1318 2023-07-13 08:57:41.740193 pushcart-0.1.9/pushcart/utils.py
+-rw-r--r--   0        0        0     2543 2023-07-13 21:42:26.395141 pushcart-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 pushcart-0.1.9/PKG-INFO
```

### Comparing `pushcart-0.1.8/LICENSE` & `pushcart-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.8/pushcart/metadata.py` & `pushcart-0.1.9/pushcart/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -381,15 +381,32 @@
         excluded_columns = (
             metadata_df.loc[tech_cols]["dest_column_name"].to_list() or None
         )
         log.info(f"Excluding technical columns: {excluded_columns}")
 
         return metadata_df.loc[~tech_cols]
 
-    def generate_code(self, keep_technical_cols: bool = False) -> set[str] | None:
+    def generate_code(self, keep_technical_cols: bool = False) -> str | None:
+        """Generate PySpark transformation code based on existing metadata.
+
+        Parameters
+        ----------
+        keep_technical_cols : bool, optional
+            Generate transformations for columns whose names start with underscore, by default False
+
+        Returns
+        -------
+        str | None
+            String containing runnable PySpark code
+
+        Raises
+        ------
+        ValueError
+            Can only generate code based on metadata that is present in memory.
+        """
         if self.metadata_df is None:
             msg = "Cannot generate PySpark code from empty metadata."
             raise ValueError(msg)
 
         mdf = self._keep_dest_cols(self.metadata_df)
 
         dest_cols = [col for col in mdf["dest_column_name"].to_list() if col] or None
@@ -406,22 +423,22 @@
         code_lines = ["df = (df"]
         for t in transformations:
             if (
                 isinstance(t["transform_function"], str)
                 and len(t["transform_function"]) > 0
             ):
                 code_lines.append(
-                    f"\t\t.withColumn(\"{t['dest_column_name']}\", {t['transform_function']})",
+                    f"\t.withColumn(\"{t['dest_column_name']}\", {t['transform_function']})",
                 )
             elif (t["source_column_name"] != t["dest_column_name"]) or (
                 t["source_column_type"] != t["dest_column_type"]
             ):
                 code_lines.append(
-                    f"\t\t.withColumn(\"{t['dest_column_name']}\", F.col(\"{t['source_column_name']}\").cast(\"{t['dest_column_type']}\"))",
+                    f"\t.withColumn(\"{t['dest_column_name']}\", F.col(\"{t['source_column_name']}\").cast(\"{t['dest_column_type']}\"))",
                 )
 
-        code_lines.append(f"\t\t.select({dest_cols}))")
-        code_str = "\n".join(code_lines)
+        code_lines.append(f"\t.select({dest_cols}))")
+        code_str = "\n" + "\n".join(code_lines)
 
         log.info(code_str)
 
         return code_str
```

### Comparing `pushcart-0.1.8/pushcart/utils.py` & `pushcart-0.1.9/pushcart/utils.py`

 * *Files identical despite different names*

### Comparing `pushcart-0.1.8/pyproject.toml` & `pushcart-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart"
-version = "0.1.8"
+version = "0.1.9"
 description = "Metadata transformations for Spark"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `pushcart-0.1.8/PKG-INFO` & `pushcart-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushcart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Metadata transformations for Spark
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

