# Comparing `tmp/func_adl-3.2.6.tar.gz` & `tmp/func_adl-3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/func_adl-3.2.6.tar", last modified: Thu Jul 13 18:10:04 2023, max compression
+gzip compressed data, was "dist/func_adl-3.2b1.tar", last modified: Sun Feb 12 10:04:09 2023, max compression
```

## Comparing `func_adl-3.2.6.tar` & `func_adl-3.2b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:10:04.000000 func_adl-3.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-13 18:10:04.000000 func_adl-3.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-13 18:09:58.000000 func_adl-3.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl/ast/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/aggregate_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/ast_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/call_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/func_adl_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/function_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/ast/syntatic_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    24078 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-13 18:09:58.000000 func_adl-3.2.6/func_adl/util_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 18:10:04.000000 func_adl-3.2.6/func_adl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 18:09:58.000000 func_adl-3.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:10:04.000000 func_adl-3.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-13 18:09:58.000000 func_adl-3.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:10:04.000000 func_adl-3.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_event_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_object_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_type_based_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_type_based_replacement_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)    20902 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_util_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-13 18:09:58.000000 func_adl-3.2.6/tests/test_util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-02-12 10:04:06.000000 func_adl-3.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/ast_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/call_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20316 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/function_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/ast/syntatic_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35230 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-12 10:04:06.000000 func_adl-3.2b1/func_adl/util_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-12 10:04:09.000000 func_adl-3.2b1/func_adl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-12 10:04:06.000000 func_adl-3.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 10:04:09.000000 func_adl-3.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-12 10:04:06.000000 func_adl-3.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 10:04:09.000000 func_adl-3.2b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_event_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_object_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_type_based_replacement_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-02-12 10:04:06.000000 func_adl-3.2b1/tests/test_util_types.py
```

### Comparing `func_adl-3.2.6/PKG-INFO` & `func_adl-3.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: func_adl
-Version: 3.2.6
+Version: 3.2b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: MIT
+License: TBD
 Platform: Any
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
```

### Comparing `func_adl-3.2.6/README.md` & `func_adl-3.2b1/README.md`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/aggregate_shortcuts.py` & `func_adl-3.2b1/func_adl/ast/aggregate_shortcuts.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/call_stack.py` & `func_adl-3.2b1/func_adl/ast/call_stack.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/func_adl_ast_utils.py` & `func_adl-3.2b1/func_adl/ast/func_adl_ast_utils.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/function_simplifier.py` & `func_adl-3.2b1/func_adl/ast/function_simplifier.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/meta_data.py` & `func_adl-3.2b1/func_adl/ast/meta_data.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/ast/syntatic_sugar.py` & `func_adl-3.2b1/func_adl/ast/syntatic_sugar.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/event_dataset.py` & `func_adl-3.2b1/func_adl/event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/functions.py` & `func_adl-3.2b1/func_adl/functions.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/object_stream.py` & `func_adl-3.2b1/func_adl/object_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import ast
-import copy
 import logging
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generic,
@@ -84,22 +83,14 @@
         """Return the query `ast` that this `ObjectStream` represents
 
         Returns:
             ast.AST: The python `ast` that is represented by this query
         """
         return self._q_ast
 
-    def clone_with_new_ast(
-        self, new_ast: ast.AST, new_type: type[S]
-    ) -> ObjectStream[S]:
-        clone = copy.deepcopy(self)
-        clone._q_ast = new_ast
-        clone._item_type = new_type
-        return clone  # type: ignore
-
     def SelectMany(
         self, func: Union[str, ast.Lambda, Callable[[T], Iterable[S]]]
     ) -> ObjectStream[S]:
         r"""
         Given the current stream's object type is an array or other iterable, return
         the items in this objects type, one-by-one. This has the effect of flattening a
         nested array.
@@ -115,18 +106,17 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(func, "SelectMany"))
+            self, _local_simplification(parse_as_ast(func))
         )
-
-        return self.clone_with_new_ast(
+        return ObjectStream[S](
             function_call("SelectMany", [n_stream.query_ast, cast(ast.AST, n_ast)]),
             unwrap_iterable(rtn_type),
         )
 
     def Select(self, f: Union[str, ast.Lambda, Callable[[T], S]]) -> ObjectStream[S]:
         r"""
         Apply a transformation function to each object in the stream, yielding a new type of
@@ -142,25 +132,20 @@
 
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
-        n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(f, "Select"))
-        )
-        return self.clone_with_new_ast(
-            function_call("Select", [n_stream.query_ast, cast(ast.AST, n_ast)]),
-            rtn_type,
+        n_stream, n_ast, rtn_type = remap_from_lambda(self, _local_simplification(parse_as_ast(f)))
+        return ObjectStream[S](
+            function_call("Select", [n_stream.query_ast, cast(ast.AST, n_ast)]), rtn_type
         )
 
-    def Where(
-        self, filter: Union[str, ast.Lambda, Callable[[T], bool]]
-    ) -> ObjectStream[T]:
+    def Where(self, filter: Union[str, ast.Lambda, Callable[[T], bool]]) -> ObjectStream[T]:
         r"""
         Filter the object stream, allowing only items for which `filter` evaluates as true through.
 
         Arguments:
 
             filter      A filter lambda that returns True/False.
 
@@ -171,31 +156,30 @@
         Notes:
             - The function can be a `lambda`, the name of a one-line function, a string that
               contains a lambda definition, or a python `ast` of type `ast.Lambda`.
         """
         from func_adl.type_based_replacement import remap_from_lambda
 
         n_stream, n_ast, rtn_type = remap_from_lambda(
-            self, _local_simplification(parse_as_ast(filter, "Where"))
+            self, _local_simplification(parse_as_ast(filter))
         )
         if rtn_type != bool:
             raise ValueError(f"The Where filter must return a boolean (not {rtn_type})")
-        return self.clone_with_new_ast(
-            function_call("Where", [n_stream.query_ast, cast(ast.AST, n_ast)]),
-            self.item_type,
+        return ObjectStream[T](
+            function_call("Where", [n_stream.query_ast, cast(ast.AST, n_ast)]), self.item_type
         )
 
     def MetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add metadata to the current object stream. The metadata is an arbitrary set of string
         key-value pairs. The backend must be able to properly interpret the metadata.
 
         Returns:
             ObjectStream: A new stream, of the same type and contents, but with metadata added.
         """
-        return self.clone_with_new_ast(
+        return ObjectStream[T](
             function_call("MetaData", [self._q_ast, as_ast(metadata)]), self.item_type
         )
 
     def QMetaData(self, metadata: Dict[str, Any]) -> ObjectStream[T]:
         """Add query metadata to the current object stream.
 
         - Metadata is never transmitted to any back end
@@ -207,35 +191,34 @@
             metadata (Dict[str, Any]): Metadata to be used later
 
         Returns:
             ObjectStream[T]: The object stream, with metadata attached
         """
         from .ast.meta_data import lookup_query_metadata
 
-        q_metadata = {}
+        first = True
+        base_ast = self.query_ast
         for k, v in metadata.items():
             found_md = lookup_query_metadata(self, k)
             add_md = False
             if found_md is None:
                 add_md = True
             elif found_md != v:
                 logging.getLogger(__name__).info(
                     f'Overwriting metadata "{k}" from its old value of "{found_md}" to "{v}"'
                 )
                 add_md = True
             if add_md:
-                q_metadata[k] = v  # type: ignore
+                if first:
+                    first = False
+                    base_ast = self.MetaData({}).query_ast
+                    base_ast._q_metadata = {}  # type: ignore
+                base_ast._q_metadata[k] = v  # type: ignore
 
-        base_ast = self.query_ast
-        if len(q_metadata) > 0:
-            new_self = self.clone_with_new_ast(copy.copy(base_ast), self.item_type)
-            new_self.query_ast._q_metadata = q_metadata  # type: ignore
-            return new_self
-        else:
-            return self.clone_with_new_ast(base_ast, self.item_type)
+        return ObjectStream[T](base_ast, self.item_type)
 
     def AsPandasDF(
         self, columns: Union[str, List[str]] = []
     ) -> ObjectStream[ReturnedDataPlaceHolder]:
         r"""
         Return a pandas stream that contains one item, an pandas `DataFrame`.
         This `DataFrame` will contain all the data fed to it. Only non-array datatypes are
@@ -285,16 +268,15 @@
             dataset.
         """
         if isinstance(columns, str):
             columns = [columns]
 
         return ObjectStream[ReturnedDataPlaceHolder](
             function_call(
-                "ResultTTree",
-                [self._q_ast, as_ast(columns), as_ast(treename), as_ast(filename)],
+                "ResultTTree", [self._q_ast, as_ast(columns), as_ast(treename), as_ast(filename)]
             )
         )
 
     as_ROOT_tree = AsROOTTTree
 
     def AsParquetFiles(
         self, filename: str, columns: Union[str, List[str]] = []
@@ -317,25 +299,23 @@
                                 suggestion.
             columns             If the data does not arrive by dictionary, then these are the
                                 column names.
 
         Returns:
 
             A new `ObjectStream` with type `[filename]`. This is because multiple files may be
-            written by the backend - the data should be concatenated together to get a final
+            written by the backend - the data should be concatinated together to get a final
             result. The order of the files back is consistent for different queries on the same
             dataset.
         """
         if isinstance(columns, str):
             columns = [columns]
 
         return ObjectStream[ReturnedDataPlaceHolder](
-            function_call(
-                "ResultParquet", [self._q_ast, as_ast(columns), as_ast(filename)]
-            )
+            function_call("ResultParquet", [self._q_ast, as_ast(columns), as_ast(filename)])
         )
 
     as_parquet = AsParquetFiles
 
     def AsAwkwardArray(
         self, columns: Union[str, List[str]] = []
     ) -> ObjectStream[ReturnedDataPlaceHolder]:
@@ -358,20 +338,19 @@
         return ObjectStream[ReturnedDataPlaceHolder](
             function_call("ResultAwkwardArray", [self._q_ast, as_ast(columns)])
         )
 
     as_awkward = AsAwkwardArray
 
     def _get_executor(
-        self,
-        executor: Optional[Callable[[ast.AST, Optional[str]], Awaitable[Any]]] = None,
+        self, executor: Optional[Callable[[ast.AST, Optional[str]], Awaitable[Any]]] = None
     ) -> Callable[[ast.AST, Optional[str]], Awaitable[Any]]:
         r"""
         Returns an executor that can be used to run this.
-        Logic separated out as it is used from several different places.
+        Logic seperated out as it is used from several different places.
 
         Arguments:
             executor            Callback to run the AST. Can be synchronous or coroutine.
 
         Returns:
             An executor that is either synchronous or a coroutine.
         """
```

### Comparing `func_adl-3.2.6/func_adl/type_based_replacement.py` & `func_adl-3.2b1/func_adl/type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/func_adl/util_ast.py` & `func_adl-3.2b1/func_adl/util_ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,22 +643,18 @@
         if len(good_lambdas) == 0:
             raise ValueError(
                 f"Internal Error - Found no lambda in source with the arguments {caller_arg_list}"
             )
 
         if len(good_lambdas) > 1:
             raise ValueError(
-                "Found multiple calls on same line"
+                "Found multiple calls to on same line"
                 + ("" if caller_name is None else f" for {caller_name}")
                 + " - split the calls across "
-                """lines or change lambda argument names so they are different. For example change:
-                    df.Select(lambda x: x + 1).Select(lambda x: x + 2)
-                    to:
-                    df.Select(lambda x: x + 1).Select(lambda y: y + 2)
-                """
+                "lines or change lambda argument names so they are different."
             )
 
         lda = good_lambdas[0]
 
     return lda
```

### Comparing `func_adl-3.2.6/func_adl/util_types.py` & `func_adl-3.2b1/func_adl/util_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import inspect
 import sys
-import typing
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 if sys.version_info >= (3, 8):
     from typing import get_args, get_origin
 else:  # pragma: no cover
     # TODO: Remove this when we drop support for 3.7
     def get_args(tp):
@@ -22,15 +21,17 @@
         t = get_inherited(t)
 
     return t is not Any
 
 
 def _is_iterable_direct(t: Type) -> bool:
     "Is this type iterable?"
-    return getattr(t, "_name", None) == "Iterable" or getattr(t, "__name__", None) == "Iterable"
+    if getattr(t, "_name", None) == "Iterable":
+        return True
+    return False
 
 
 def get_inherited(t: Type) -> Type:
     """Returns the inherited type of `t`
 
     Notes:
     * This works for 3.7 forward (but not back!)
@@ -49,26 +50,15 @@
         return Any
 
     r = base_classes[0]  # type: ignore
 
     g_args = get_args(t)
     if len(g_args) > 0:
         mapping = {a.__name__: v for a, v in zip(r.__parameters__, g_args)}
-
-        r_base = get_origin(r)
-        assert r_base is not None, "Internal error"
-
-        # Get us back to typing if this is a common interface.
-        # This is not needed in python 3.11 and forward, where
-        # collections.abc.X can are all be parameterized.
-        if r_base.__name__ in typing.__dict__:
-            r_base = typing.__dict__[r_base.__name__]
-
-        # Re-parameterize the type with the information e have from this parameterization.
-        r = r_base[tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))]
+        r.__args__ = tuple(_resolve_type(t_arg, mapping) for t_arg in get_args(r))
 
     return r
 
 
 def unwrap_iterable(t: Type) -> Type:
     "Unwrap an iterable type"
     # Try to find an iterable in the history somehow
@@ -123,15 +113,15 @@
     Args:
         t (Type): The type to resolve
         parameters (Dict[str, Type]): The dict of types to resolve
 
     Returns:
         None if `t` is parameterized by unknown type var's
         The resolved type (a copy leaving `t` untouched) if TypeVar's are filled in
-        The type if no substitution is required.
+        The type if no substition is required.
     """
     if isinstance(t, TypeVar):
         if t.__name__ in parameters:
             return parameters[t.__name__]
         return None
 
     template_params = getattr(t, "__parameters__", None)
```

### Comparing `func_adl-3.2.6/func_adl.egg-info/PKG-INFO` & `func_adl-3.2b1/func_adl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: func-adl
-Version: 3.2.6
+Version: 3.2b1
 Summary: Functional Analysis Description Language Base Package
 Home-page: https://github.com/iris-hep/func_adl
 Author: G. Watts (IRIS-HEP/UW Seattle)
 Author-email: gwatts@uw.edu
 Maintainer: Gordon Watts (IRIS-HEP/UW Seattle)
 Maintainer-email: gwatts@uw.edu
-License: MIT
+License: TBD
 Platform: Any
-Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
```

### Comparing `func_adl-3.2.6/func_adl.egg-info/SOURCES.txt` & `func_adl-3.2b1/func_adl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/setup.py` & `func_adl-3.2b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,35 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="G. Watts (IRIS-HEP/UW Seattle)",
     author_email="gwatts@uw.edu",
     maintainer="Gordon Watts (IRIS-HEP/UW Seattle)",
     maintainer_email="gwatts@uw.edu",
     url="https://github.com/iris-hep/func_adl",
-    license="MIT",
+    license="TBD",
     test_suite="tests",
     install_requires=["make-it-sync"],
     setup_requires=["pytest-runner"],
     tests_require=["pytest>=3.9"],
     extras_require=extras_require,
     classifiers=[
         # "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
-        "Development Status :: 5 - Production/Stable",
+        # "Development Status :: 5 - Production/Stable",
         # "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.6",
         "Topic :: Software Development",
         "Topic :: Utilities",
     ],
     data_files=[],
     python_requires=">=3.6, <3.12",
     platforms="Any",
 )
```

### Comparing `func_adl-3.2.6/tests/test_event_dataset.py` & `func_adl-3.2b1/tests/test_event_dataset.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/tests/test_object_stream.py` & `func_adl-3.2b1/tests/test_object_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Test the object stream
 import ast
 import asyncio
 import logging
-from _ast import Call
 from typing import Any, Iterable, Optional, Tuple, TypeVar
 
 import pytest
 
 from func_adl import EventDataset
 from func_adl.object_stream import ObjectStream
 from func_adl.type_based_replacement import func_adl_callback
@@ -31,17 +30,15 @@
     def eta(self) -> float:
         ...
 
 
 T = TypeVar("T")
 
 
-def add_md_for_type(
-    s: ObjectStream[T], a: ast.Call
-) -> Tuple[ObjectStream[T], ast.Call]:
+def add_md_for_type(s: ObjectStream[T], a: ast.Call) -> Tuple[ObjectStream[T], ast.Call]:
     return s.MetaData({"hi": "there"}), a
 
 
 @func_adl_callback(add_md_for_type)
 class dd_event:
     def Jets(self, bank: str) -> Iterable[dd_jet]:
         ...
@@ -74,20 +71,14 @@
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
     )
     assert isinstance(r, ast.AST)
 
 
-def test_simple_query_one_line():
-    """Make sure we parse 2 functions on one line correctly"""
-    r = my_event().Select(lambda e: e.met).Where(lambda e: e > 10).value()
-    assert isinstance(r, ast.AST)
-
-
 def test_two_simple_query():
     r1 = (
         my_event()
         .SelectMany("lambda e: e.jets()")
         .Select("lambda j: j.pT()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
@@ -297,39 +288,18 @@
 
     assert lookup_query_metadata(r1, "two") == "2"
     assert lookup_query_metadata(r2, "two") == "2+"
 
     assert len(caplog.text) == 0
 
 
-def test_query_metadata_not_empty():
-    r_base = my_event().QMetaData({"one": "1"})
-    q_ast = r_base.query_ast
-
-    class MDScanner(ast.NodeVisitor):
-        def visit_Call(self, node: Call) -> Any:
-            if not isinstance(node.func, ast.Name):
-                return self.generic_visit(node)
-            if node.func.id != "MetaData":
-                return self.generic_visit(node)
-            assert len(node.args) == 2
-            md_dict = node.args[1]
-            assert isinstance(md_dict, ast.Dict)
-            assert len(md_dict.keys) > 0
-            return self.generic_visit(node)
-
-    MDScanner().visit(q_ast)
-
-
 def test_nested_query_rendered_correctly():
     r = (
         my_event()
-        .Where(
-            "lambda e: e.jets.Select(lambda j: j.pT()).Where(lambda j: j > 10).Count() > 0"
-        )
+        .Where("lambda e: e.jets.Select(lambda j: j.pT()).Where(lambda j: j > 10).Count() > 0")
         .SelectMany("lambda e: e.jets()")
         .AsROOTTTree("junk.root", "analysis", "jetPT")
         .value()
     )
     assert isinstance(r, ast.AST)
     assert "Select(source" not in ast.dump(r)
```

### Comparing `func_adl-3.2.6/tests/test_type_based_replacement.py` & `func_adl-3.2b1/tests/test_type_based_replacement.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/tests/test_type_based_replacement_py310.py` & `func_adl-3.2b1/tests/test_type_based_replacement_py310.py`

 * *Files identical despite different names*

### Comparing `func_adl-3.2.6/tests/test_util_ast.py` & `func_adl-3.2b1/tests/test_util_ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -678,46 +678,14 @@
         .value()
     )
     # fmt: on
     assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
     assert "uncalibrated_collection" in ast.dump(found[0])
 
 
-def test_parse_select_where():
-    "Common lambas with different parent functions on one line - found in wild"
-
-    found = []
-
-    class my_obj:
-        def Where(self, x: Callable):
-            found.append(parse_as_ast(x, "Where"))
-            return self
-
-        def Select(self, x: Callable):
-            found.append(parse_as_ast(x, "Select"))
-            return self
-
-        def AsAwkwardArray(self, stuff: str):
-            return self
-
-        def value(self):
-            return self
-
-    jets_pflow_name = "hi"
-    ds_dijet = my_obj()
-
-    # fmt: off
-    jets_pflow = (
-        ds_dijet.Select(lambda e: e.met).Where(lambda e: e > 100)
-    )
-    # fmt: on
-    assert jets_pflow is not None  # Just to keep flake8 happy without adding a noqa above.
-    assert "met" in ast.dump(found[0])
-
-
 def test_parse_multiline_lambda_ok_with_one_as_arg():
     "Make sure we can properly parse a multi-line lambda - but now with argument"
 
     found = []
 
     class my_obj:
         def do_it(self, x: Callable, counter: int):
```

### Comparing `func_adl-3.2.6/tests/test_util_types.py` & `func_adl-3.2b1/tests/test_util_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     T = TypeVar("T")
 
     class bogus(Iterable[T]):
         pass
 
     myc = bogus[int]
 
-    assert get_inherited(myc) == Iterable[int]  # type: ignore
+    assert get_inherited(myc) == Iterable[int]
 
 
 def test_get_inherited_two_levels():
     T = TypeVar("T")
     U = TypeVar("U")
 
     class bogus(Generic[T]):
@@ -102,27 +102,14 @@
     class bogus2(bogus[Iterable[U]]):
         pass
 
     myc = bogus2[int]
     assert get_inherited(myc) == bogus[Iterable[int]]
 
 
-def test_get_inherited_generic_twice():
-    T = TypeVar("T")
-
-    class bogus(Iterable[T]):
-        pass
-
-    myc = bogus[int]
-    assert get_inherited(myc) == Iterable[int]  # type: ignore
-
-    myd = bogus[float]
-    assert get_inherited(myd) == Iterable[float]  # type: ignore
-
-
 def test_build_type_int():
     assert build_type_dict_from_type(int) == {}
 
 
 def test_build_type_generic():
     T = TypeVar("T")
```

