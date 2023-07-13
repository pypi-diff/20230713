# Comparing `tmp/unit_syntax-0.1.6.tar.gz` & `tmp/unit_syntax-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.1.6.tar", max compression
+gzip compressed data, was "unit_syntax-0.1.7.tar", max compression
```

## Comparing `unit_syntax-0.1.6.tar` & `unit_syntax-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5284 2023-07-12 20:25:13.148092 unit_syntax-0.1.6/README.md
--rw-r--r--   0        0        0      641 2023-07-12 20:25:13.148092 unit_syntax-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2159 2023-07-12 20:25:13.148092 unit_syntax-0.1.6/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149367 2023-07-12 20:25:13.152092 unit_syntax-0.1.6/unit_syntax/parser.py
--rw-r--r--   0        0        0     5039 2023-07-12 20:25:13.152092 unit_syntax-0.1.6/unit_syntax/transform.py
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 unit_syntax-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5284 2023-07-12 20:35:54.445118 unit_syntax-0.1.7/README.md
+-rw-r--r--   0        0        0      641 2023-07-12 20:35:54.445118 unit_syntax-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2392 2023-07-12 20:35:54.445118 unit_syntax-0.1.7/unit_syntax/__init__.py
+-rw-r--r--   0        0        0   149367 2023-07-12 20:35:54.445118 unit_syntax-0.1.7/unit_syntax/parser.py
+-rw-r--r--   0        0        0     5039 2023-07-12 20:35:54.445118 unit_syntax-0.1.7/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 unit_syntax-0.1.7/PKG-INFO
```

### Comparing `unit_syntax-0.1.6/README.md` & `unit_syntax-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.6/pyproject.toml` & `unit_syntax-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.1.6"
+version = "0.1.7"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{include = "unit_syntax"}]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
 description = "Physical unit literals for Jupyter and IPython"
 
 [tool.poetry.dependencies]
```

### Comparing `unit_syntax-0.1.6/unit_syntax/__init__.py` & `unit_syntax-0.1.7/unit_syntax/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,19 +52,29 @@
     else:
         do_transform = transform_lines
     ip.input_transformers_post.append(do_transform)
 
     # Overide default formatters to use reduced units.  This lets us keep using the
     # default registry for interop with other pint-using libraries, but gives more
     # sensible output in the notebook.
-    def add_formatter(mime, fn):
-        formatter = ip.display_formatter.formatters[mime]
-        formatter.for_type(pint.Quantity, fn)
-
-    add_formatter("text/markdown", _format_quantity_markdown)
-    add_formatter("text/html", _format_quantity_html)
-    add_formatter("text/plain", _format_quantity_pretty)
-    add_formatter("text/latex", _format_quantity_latex)
+    def add_formatter(mime, display_fn_name):
+        formatter = ip.display_formatter.formatters.get(mime)
+        if formatter is None:
+            return
+
+        fn = getattr(pint.Quantity, display_fn_name, None)
+        if fn is None:
+            return
+
+        def fmt_reduced(q, *args):
+            return fn(q.to_reduced_units(), *args)
+
+        formatter.for_type(pint.Quantity, fmt_reduced)
+
+    add_formatter("text/markdown", "_repr_markdown_")
+    add_formatter("text/html", "_repr_html_")
+    add_formatter("text/plain", "_repr_pretty_")
+    add_formatter("text/latex", "_repr_latex_")
 
     # ensure the module is still visible if imported via
     # `from unit_syntax import ipython` for some reason
     ip.run_cell("import unit_syntax")
```

### Comparing `unit_syntax-0.1.6/unit_syntax/parser.py` & `unit_syntax-0.1.7/unit_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.6/unit_syntax/transform.py` & `unit_syntax-0.1.7/unit_syntax/transform.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.6/PKG-INFO` & `unit_syntax-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.1.6
+Version: 0.1.7
 Summary: Physical unit literals for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

