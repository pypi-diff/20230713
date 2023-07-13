# Comparing `tmp/dask_awkward-2023.7.0.tar.gz` & `tmp/dask_awkward-2023.7.1.tar.gz`

## Comparing `dask_awkward-2023.7.0.tar` & `dask_awkward-2023.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    76062 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    16603 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    28922 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/README.md
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dask_awkward-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    76062 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    29197 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/README.md
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/PKG-INFO
```

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.7.1/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/typing.py` & `dask_awkward-2023.7.1/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/utils.py` & `dask_awkward-2023.7.1/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.7.1/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/core.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/core.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,16 +385,16 @@
     # now we try to compute for each possible output layer key (leaf
     # node on partition 0); this will cause the typetacer reports to
     # get correct fields/columns touched. If the result is a record or
     # an array we of course want to touch all of the data/fields.
     try:
         for layer in hlg.layers.values():
             layer.__dict__.pop("_cached_dict", None)
-        for outlayerkey in leaf_layers_keys:
-            out = get_sync(hlg, outlayerkey)
+        results = get_sync(hlg, leaf_layers_keys)
+        for out in results:
             if isinstance(out, (ak.Array, ak.Record)):
                 out.layout._touch_data(recursive=True)
     except Exception as err:
         on_fail = dask.config.get("awkward.optimization.on-fail")
         # this is the default, throw a warning but skip the optimization.
         if on_fail == "warn":
             warnings.warn(
```

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,21 @@
 
 
 class _ArgCartesianFn:
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def __call__(self, *arrays):
+        # FIXME: with proper typetracer/form rehydration support we
+        # should not need to manually touch this when it's a
+        # typetracer
+        for a in arrays:
+            if ak.backend(a) == "typetracer":
+                a.layout._touch_data(recursive=True)
+
         return ak.argcartesian(list(arrays), **self.kwargs)
 
 
 @borrow_docstring(ak.argcartesian)
 def argcartesian(
     arrays,
     axis=1,
```

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/unproject_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,17 @@
     # handle other cases that come up here...
 
     else:
         raise AssertionError(f"unexpected combination: {type(form)} and {type(layout)}")
 
 
 def unproject_layout(form: Form | None, layout: Content) -> Content:
-    """Rehydrate a layout to include all parts of an original form.
+    """Does nothing! Currently returns the passed in layout unchanged!
+
+    Rehydrate a layout to include all parts of an original form.
 
     When we perform the necessary columns optimization we drop fields
     that are not necessary for a computed result. Sometimes we have
     task graphs that expect to see fields in name only (but no their
     data). To protect against FieldNotFound exception we "unproject"
     or "rehydrate" the layout with the original form. This reapplys
     all original fields, but the ones that were orignally projected
@@ -397,10 +399,11 @@
     Returns
     -------
     awkward.contents.content.Content
         Unprojected layout (all fields from the original form that did
         not appear in the projected layout will be PlaceholderArrays).
 
     """
-    if form is None:
-        return layout
-    return _unproject_layout(form, layout, layout.length, layout.backend)
+    return layout
+    # if form is None:
+    #     return layout
+    # return _unproject_layout(form, layout, layout.length, layout.backend)
```

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.7.1/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/.gitignore` & `dask_awkward-2023.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/LICENSE` & `dask_awkward-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/README.md` & `dask_awkward-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.0/pyproject.toml` & `dask_awkward-2023.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "pyarrow",
 ]
 complete = [
   "dask-awkward[io]",
 ]
 # `docs` and `test` are separate from user installs
 docs = [
-  "dask-awkard[complete]",
+  "dask-awkward[complete]",
   "dask-sphinx-theme >=3.0.2",
   "sphinx-design",
   "requests >=2.27.1",
 ]
 test = [
   "dask-awkward[complete]",
   "distributed",
@@ -145,14 +145,15 @@
   "\\.\\.\\.$",
 ]
 fail_under = 90
 show_missing = true
 
 [tool.coverage.run]
 omit = [
+  "*/dask_awkward/lib/unproject_layout.py",
   "*/tests/test_*.py",
   "*/tests/__init__.py",
   "*/version.py",
 ]
 source = ["src/"]
 
 [tool.ruff]
```

### Comparing `dask_awkward-2023.7.0/PKG-INFO` & `dask_awkward-2023.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: awkward>=2.2.4
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: dask-awkward[io]; extra == 'complete'
 Provides-Extra: docs
-Requires-Dist: dask-awkard[complete]; extra == 'docs'
+Requires-Dist: dask-awkward[complete]; extra == 'docs'
 Requires-Dist: dask-sphinx-theme>=3.0.2; extra == 'docs'
 Requires-Dist: requests>=2.27.1; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Provides-Extra: io
 Requires-Dist: aiohttp; extra == 'io'
 Requires-Dist: pyarrow; extra == 'io'
 Provides-Extra: test
```

