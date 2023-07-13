# Comparing `tmp/abi3info-2023.7.11.tar.gz` & `tmp/abi3info-2023.7.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2023.7.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "abi3info-2023.7.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `abi3info-2023.7.11.tar` & `abi3info-2023.7.13.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-07-12 01:00:39.921742 abi3info-2023.7.11/LICENSE
--rw-r--r--   0        0        0     1915 2023-07-12 01:00:39.921742 abi3info-2023.7.11/README.md
--rw-r--r--   0        0        0     1038 2023-07-12 01:00:39.921742 abi3info-2023.7.11/abi3info/__init__.py
--rw-r--r--   0        0        0   190499 2023-07-12 01:00:39.921742 abi3info-2023.7.11/abi3info/_internal.py
--rw-r--r--   0        0        0     7791 2023-07-12 01:00:39.921742 abi3info-2023.7.11/abi3info/models.py
--rw-r--r--   0        0        0     1885 2023-07-12 01:00:39.921742 abi3info-2023.7.11/pyproject.toml
--rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 abi3info-2023.7.11/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-07-13 05:01:38.633352 abi3info-2023.7.13/LICENSE
+-rw-r--r--   0        0        0     1915 2023-07-13 05:01:38.633352 abi3info-2023.7.13/README.md
+-rw-r--r--   0        0        0     1038 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/__init__.py
+-rw-r--r--   0        0        0   191351 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/_internal.py
+-rw-r--r--   0        0        0     7791 2023-07-13 05:01:38.633352 abi3info-2023.7.13/abi3info/models.py
+-rw-r--r--   0        0        0     1885 2023-07-13 05:01:38.633352 abi3info-2023.7.13/pyproject.toml
+-rw-r--r--   0        0        0     3462 1970-01-01 00:00:00.000000 abi3info-2023.7.13/PKG-INFO
```

### Comparing `abi3info-2023.7.11/LICENSE` & `abi3info-2023.7.13/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.11/README.md` & `abi3info-2023.7.13/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.11/abi3info/__init__.py` & `abi3info-2023.7.13/abi3info/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2023.07.11"
+__version__ = "2023.07.13"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2023.7.11/abi3info/_internal.py` & `abi3info-2023.7.13/abi3info/_internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -4457,14 +4457,38 @@
     ),
     Symbol(name="PyObject_DelAttrString"): Function(
         symbol=Symbol(name="PyObject_DelAttrString"),
         added=PyVersion(major=3, minor=13),
         ifdef=None,
         abi_only=False,
     ),
+    Symbol(name="PyObject_GetOptionalAttr"): Function(
+        symbol=Symbol(name="PyObject_GetOptionalAttr"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
+    ),
+    Symbol(name="PyObject_GetOptionalAttrString"): Function(
+        symbol=Symbol(name="PyObject_GetOptionalAttrString"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
+    ),
+    Symbol(name="PyMapping_GetOptionalItem"): Function(
+        symbol=Symbol(name="PyMapping_GetOptionalItem"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
+    ),
+    Symbol(name="PyMapping_GetOptionalItemString"): Function(
+        symbol=Symbol(name="PyMapping_GetOptionalItemString"),
+        added=PyVersion(major=3, minor=13),
+        ifdef=None,
+        abi_only=False,
+    ),
 }
 _MACROS: Final[dict[str, Macro]] = {
     "Py_tp_dealloc": Macro(name="Py_tp_dealloc", added=PyVersion(major=3, minor=2)),
     "Py_tp_getattr": Macro(name="Py_tp_getattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_setattr": Macro(name="Py_tp_setattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_repr": Macro(name="Py_tp_repr", added=PyVersion(major=3, minor=2)),
     "Py_tp_hash": Macro(name="Py_tp_hash", added=PyVersion(major=3, minor=2)),
```

### Comparing `abi3info-2023.7.11/abi3info/models.py` & `abi3info-2023.7.13/abi3info/models.py`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.11/pyproject.toml` & `abi3info-2023.7.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2023.7.11/PKG-INFO` & `abi3info-2023.7.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2023.7.11
+Version: 2023.7.13
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

