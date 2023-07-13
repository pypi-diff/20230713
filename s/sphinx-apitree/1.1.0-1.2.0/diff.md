# Comparing `tmp/sphinx_apitree-1.1.0.tar.gz` & `tmp/sphinx_apitree-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_apitree-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_apitree-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_apitree-1.1.0.tar` & `sphinx_apitree-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/LICENSE
--rw-r--r--   0        0        0     1980 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/README.md
--rw-r--r--   0        0        0      105 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/__init__.py
--rw-r--r--   0        0        0     1338 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ast_utils.py
--rw-r--r--   0        0        0     2723 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/conf_util.py
--rw-r--r--   0        0        0      761 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ext/docstring.py
--rw-r--r--   0        0        0      443 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/ext/linkify.py
--rw-r--r--   0        0        0     1691 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/html_helper.py
--rw-r--r--   0        0        0       30 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/main.py
--rw-r--r--   0        0        0      330 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/md_utils.py
--rw-r--r--   0        0        0      164 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/signature_utils.py
--rw-r--r--   0        0        0      446 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/structs.py
--rw-r--r--   0        0        0     9597 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/symbol_match.py
--rw-r--r--   0        0        0      183 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/api.md
--rw-r--r--   0        0        0       13 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/attribute.md
--rw-r--r--   0        0        0      144 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/class.md
--rw-r--r--   0        0        0       73 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/function.md
--rw-r--r--   0        0        0      154 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/module.md
--rw-r--r--   0        0        0       13 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/templates/type_alias.md
--rw-r--r--   0        0        0     1693 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/tree_extractor.py
--rw-r--r--   0        0        0      782 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/apitree/writer.py
--rw-r--r--   0        0        0     1508 2023-07-11 15:10:13.972805 sphinx_apitree-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 sphinx_apitree-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1980 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/README.md
+-rw-r--r--   0        0        0      105 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/__init__.py
+-rw-r--r--   0        0        0     1338 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ast_utils.py
+-rw-r--r--   0        0        0     4146 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/conf_util.py
+-rw-r--r--   0        0        0      761 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ext/docstring.py
+-rw-r--r--   0        0        0      443 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/ext/linkify.py
+-rw-r--r--   0        0        0     1691 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/html_helper.py
+-rw-r--r--   0        0        0       30 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/main.py
+-rw-r--r--   0        0        0      330 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/md_utils.py
+-rw-r--r--   0        0        0      164 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/signature_utils.py
+-rw-r--r--   0        0        0      446 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/structs.py
+-rw-r--r--   0        0        0     9597 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/symbol_match.py
+-rw-r--r--   0        0        0      183 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/api.md
+-rw-r--r--   0        0        0       13 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/attribute.md
+-rw-r--r--   0        0        0      144 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/class.md
+-rw-r--r--   0        0        0       73 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/function.md
+-rw-r--r--   0        0        0      154 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/module.md
+-rw-r--r--   0        0        0       13 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/templates/type_alias.md
+-rw-r--r--   0        0        0     1693 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/tree_extractor.py
+-rw-r--r--   0        0        0      782 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/apitree/writer.py
+-rw-r--r--   0        0        0     1508 2023-07-13 10:12:27.566413 sphinx_apitree-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 sphinx_apitree-1.2.0/PKG-INFO
```

### Comparing `sphinx_apitree-1.1.0/LICENSE` & `sphinx_apitree-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/README.md` & `sphinx_apitree-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/ast_utils.py` & `sphinx_apitree-1.2.0/apitree/ast_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/ext/docstring.py` & `sphinx_apitree-1.2.0/apitree/ext/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/html_helper.py` & `sphinx_apitree-1.2.0/apitree/html_helper.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/symbol_match.py` & `sphinx_apitree-1.2.0/apitree/symbol_match.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/tree_extractor.py` & `sphinx_apitree-1.2.0/apitree/tree_extractor.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/apitree/writer.py` & `sphinx_apitree-1.2.0/apitree/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/pyproject.toml` & `sphinx_apitree-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_apitree-1.1.0/PKG-INFO` & `sphinx_apitree-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-apitree
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sphinx extension to auto-generate API tree.
 Keywords: sphinx,doc
 Author-email: Conchylicultor <etiennefg.pot@mail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

