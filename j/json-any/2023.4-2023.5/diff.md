# Comparing `tmp/json-any-2023.4.tar.gz` & `tmp/json-any-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.4.tar", last modified: Wed Jul 12 16:20:20 2023, max compression
+gzip compressed data, was "json-any-2023.5.tar", last modified: Thu Jul 13 13:56:27 2023, max compression
```

## Comparing `json-any-2023.4.tar` & `json-any-2023.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.4/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 16:20:20.027000 json-any-2023.4/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.4/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.4/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.023667 json-any-2023.4/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.4/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1754 2023-07-11 10:57:55.000000 json-any-2023.4/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.4/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     2848 2023-07-11 10:24:57.000000 json-any-2023.4/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     2895 2023-07-11 10:56:35.000000 json-any-2023.4/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     6528 2023-07-11 09:47:11.000000 json-any-2023.4/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     4259 2023-07-11 15:42:31.000000 json-any-2023.4/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11674 2023-07-12 16:06:38.000000 json-any-2023.4/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    13809 2023-07-12 16:07:02.000000 json-any-2023.4/json_any/object_to_json.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-12 16:17:18.000000 json-any-2023.4/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-12 16:20:20.027000 json-any-2023.4/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-12 16:20:20.000000 json-any-2023.4/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.4/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-12 16:20:20.027000 json-any-2023.4/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.4/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.5/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 13:56:27.843092 json-any-2023.5/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.5/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.5/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.839759 json-any-2023.5/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.5/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.5/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.5/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     4597 2023-07-13 13:50:35.000000 json-any-2023.5/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.5/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.5/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     4245 2023-07-13 13:14:00.000000 json-any-2023.5/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11912 2023-07-13 13:42:10.000000 json-any-2023.5/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    12700 2023-07-13 13:46:55.000000 json-any-2023.5/json_any/object_to_json.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-13 13:53:47.000000 json-any-2023.5/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-13 13:56:27.843092 json-any-2023.5/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      461 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-13 13:56:27.000000 json-any-2023.5/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.5/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-13 13:56:27.843092 json-any-2023.5/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5293 2023-07-11 12:01:48.000000 json-any-2023.5/setup.py
```

### Comparing `json-any-2023.4/PKG-INFO` & `json-any-2023.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.4
+Version: 2023.5
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.4/README-LICENCE-utf8.txt` & `json-any-2023.5/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.4/README.rst` & `json-any-2023.5/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2023.4/documentation/wiki/description.asciidoc` & `json-any-2023.5/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.4/json_any/__init__.py` & `json-any-2023.5/json_any/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from json_any.extension.type import FullyQualifiedType
+from json_any.extension.type import QualifiedType
 from json_any.json_to_object import ObjectFromJsonString
 from json_any.object_to_json import JsonStringOf
 from json_any.version import __version__
```

### Comparing `json-any-2023.4/json_any/catalog/module.py` & `json-any-2023.5/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.4/json_any/catalog/type.py` & `json-any-2023.5/json_any/constant.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,52 +25,18 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from array import array as py_array_t
-from datetime import date as date_t
-from datetime import datetime as date_time_t
-from datetime import time as time_t
-from datetime import timedelta as time_delta_t
-from datetime import timezone as time_zone_t
-from enum import Enum as enum_t
-from io import BytesIO as io_bytes_t
-from pathlib import PurePath as path_t
-from typing import NamedTuple as named_tuple_t
-from uuid import UUID as uuid_t
+DESCRIPTION_FOR_JSON = "__DescriptionForJSON__"
+NEW_FROM_JSON_DESCRIPTION = "__NewFromJsonDescription__"
 
-from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs
+CUSTOM_PREFIX = "CUSTOM_"
+DATACLASS_PREFIX = "DATACLASS_"
+STANDARD_PREFIX = "STANDARD_"
+UNHANDLED_PREFIX = "UNHANDLED_"
 
-# When a module is not found, using bytes, the first type tested while JSONing, as the main module type is a safe way to
-# "disable" it.
-if pypl is None:
-    figure_t = bytes
-else:
-    figure_t = pypl.Figure
-if grph is None:
-    NX_GRAPH_CLASSES = bytes
-else:
-    NX_GRAPH_CLASSES = (grph.Graph, grph.DiGraph, grph.MultiGraph, grph.MultiDiGraph)
-if nmpy is None:
-    array_t = bytes
-else:
-    array_t = nmpy.ndarray
-if pnds is None:
-    series_t = data_frame_t = bytes
-else:
-    series_t = pnds.Series
-    data_frame_t = pnds.DataFrame
-if sprs is None:
-    SPARSE_ARRAY_CLASSES = bytes
-else:
-    SPARSE_ARRAY_CLASSES = (
-        sprs.bsr_array,
-        sprs.coo_array,
-        sprs.csc_array,
-        sprs.csr_array,
-        sprs.dia_array,
-        sprs.dok_array,
-        sprs.lil_array,
-    )
+MODULE_TYPE_SEPARATOR = ":"  # Must be a character forbidden in any Python token.
+
+JSONING_ERROR_MARKER = "/!\\"
```

### Comparing `json-any-2023.4/json_any/extension/numpy.py` & `json-any-2023.5/json_any/extension/numpy.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,154 +26,194 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import json
-from typing import Callable
+from typing import Any, Callable
 
 from json_any.catalog.module import blsc, nmpy, pcst
-from json_any.catalog.type import array_t, io_bytes_t
+from json_any.catalog.type import io_bytes_t
+from json_any.catalog.type import np_array_t as array_t
+
+BLOSC = "blosc"
+BLOSC_BYTES = "blosc.bytes"
+NUMPY = "numpy"
+NUMPY_COMPRESSED = "numpy.compressed"
+PCA_B_STREAM = "pca_b_stream"
 
-_BLOSC_BYTES_VERSION = "blosc.bytes"
-_BLOSC_VERSION = "blosc"
-_NUMPY_COMPRESSED_VERSION = "compressed"
 _NUMPY_NDARRAY_FROM_VERSIONS = {}
 _NUMPY_NDARRAY_TO_VERSIONS = {}
-_NUMPY_PLAIN_VERSION = "plain"
-_PCA_B_STREAM_VERSION = "pca_b_stream"
 
+if nmpy is None:
+
+    def _RaiseException() -> None:
+        """"""
+        raise NotImplementedError(f"Numpy module not installed or importable.")
+
+    def IsNumpyScalar(*_, **__) -> Any:
+        _RaiseException()
+
+    def AsScalarRepresentation(*_, **__) -> Any:
+        _RaiseException()
+
+    def AsMostConciseRepresentation(*_, **__) -> Any:
+        _RaiseException()
+
+    def AsNumpyArray(*_, **__) -> Any:
+        _RaiseException()
+
+    def AddNumpyNDArrayRepresentation(*_, **__) -> None:
+        _RaiseException()
+
+    def RemoveNumpyNDArrayRepresentation(*_, **__) -> None:
+        _RaiseException()
+
+else:
+    _SCALAR_META_TYPES = (nmpy.bool_, nmpy.number, nmpy.character)
+
+    def IsNumpyScalar(type_: type, /) -> bool:
+        """"""
+        return nmpy.issubclass_(type_, _SCALAR_META_TYPES)
+
+    def AsScalarRepresentation(instance: Any, type_: type, /) -> Any:
+        """"""
+        if nmpy.issubclass_(type_, nmpy.bool_):
+            output = bool(instance)
+        elif nmpy.issubclass_(type_, nmpy.integer):
+            output = int(instance)
+        elif nmpy.issubclass_(type_, nmpy.floating):
+            output = float(instance)
+        elif nmpy.issubclass_(type_, complex):
+            # Use list (instead of tuple) since tuples seem to be unJSONed as list, so...
+            output = [float(nmpy.real(instance)), float(nmpy.imag(instance))]
+        else:
+            output = str(instance)
 
-def AsMostConciseRepresentation(array: array_t, /) -> tuple[str, str]:
-    """"""
-    version = (array.tolist(), array.dtype.char)
-    try:
-        min_length = json.dumps(version).__len__()
-        output = (_NUMPY_PLAIN_VERSION, version)
-    except TypeError:
-        min_length = None
-        output = ("None", None)
-
-    fake_file = io_bytes_t()
-    nmpy.savez_compressed(fake_file, array=array)
-    version = fake_file.getvalue().decode(encoding="iso-8859-1")
-    fake_file.close()
-    length = version.__len__()
-    if (min_length is None) or (length < min_length):
-        output, min_length = (_NUMPY_COMPRESSED_VERSION, version), length
-
-    for ToVersion in _NUMPY_NDARRAY_TO_VERSIONS.values():
-        version = ToVersion(array)
-        if version is None:
-            continue
-        length = version[1].__len__()
-        if length < min_length:
-            output, min_length = version, length
-
-    return output
-
-
-def AsNumpyArray(how: str, what: str) -> array_t:
-    """"""
-    if how == _NUMPY_PLAIN_VERSION:
-        data, dtype = what
-        return nmpy.array(data, dtype=dtype)
-    elif how == _NUMPY_COMPRESSED_VERSION:
-        fake_file = io_bytes_t(what.encode(encoding="iso-8859-1"))
-        output = nmpy.load(fake_file)["array"]
-        fake_file.close()
         return output
 
-    return _NUMPY_NDARRAY_FROM_VERSIONS[how](what)
+    def AsMostConciseRepresentation(array: array_t, /) -> tuple[str, str]:
+        """"""
+        version = (array.tolist(), array.dtype.char)
+        try:
+            min_length = json.dumps(version).__len__()
+            output = (NUMPY, version)
+        except TypeError:
+            min_length = None
+            output = ("None", None)
+
+        fake_file = io_bytes_t()
+        nmpy.savez_compressed(fake_file, array=array)
+        version = fake_file.getvalue().decode(encoding="iso-8859-1")
+        fake_file.close()
+        length = version.__len__()
+        if (min_length is None) or (length < min_length):
+            output, min_length = (NUMPY_COMPRESSED, version), length
+
+        for ToVersion in _NUMPY_NDARRAY_TO_VERSIONS.values():
+            version = ToVersion(array)
+            if version is None:
+                continue
+            length = version[1].__len__()
+            if length < min_length:
+                output, min_length = version, length
 
+        return output
 
-def AddNumpyNDArrayRepresentation(
-    name: str,
-    /,
-    *,
-    ToVersion: Callable[[array_t], tuple[int, str, str]] = None,
-    FromVersion: Callable[[str], array_t] = None,
-) -> None:
-    """"""
-    global _NUMPY_NDARRAY_TO_VERSIONS, _NUMPY_NDARRAY_FROM_VERSIONS
-
-    if name in (_NUMPY_PLAIN_VERSION, _NUMPY_COMPRESSED_VERSION):
-        raise ValueError(
-            f"{_NUMPY_PLAIN_VERSION}, {_NUMPY_COMPRESSED_VERSION}: Reserved representation names"
-        )
-
-    if name == _BLOSC_VERSION:
-        if blsc is None:
-            raise ModuleNotFoundError('Module "blosc" not installed or unfoundable')
-        _NUMPY_NDARRAY_TO_VERSIONS[_BLOSC_VERSION] = _BloscVersion
-        _NUMPY_NDARRAY_FROM_VERSIONS[_BLOSC_VERSION] = _FromBloscVersion
-        _NUMPY_NDARRAY_FROM_VERSIONS[_BLOSC_BYTES_VERSION] = _FromBloscBytesVersion
-    elif name == _PCA_B_STREAM_VERSION:
-        if pcst is None:
-            raise ModuleNotFoundError(
-                'Module "pca_b_stream" not installed or unfoundable'
-            )
-        _NUMPY_NDARRAY_TO_VERSIONS[_PCA_B_STREAM_VERSION] = _PCABStreamVersion
-        _NUMPY_NDARRAY_FROM_VERSIONS[_PCA_B_STREAM_VERSION] = _FromPCABStreamVersion
-    else:
-        if (ToVersion is None) or (FromVersion is None):
+    def AsNumpyArray(how: str, what: str) -> array_t:
+        """"""
+        if how == NUMPY:
+            data, dtype = what
+            return nmpy.array(data, dtype=dtype)
+        elif how == NUMPY_COMPRESSED:
+            fake_file = io_bytes_t(what.encode(encoding="iso-8859-1"))
+            output = nmpy.load(fake_file)["array"]
+            fake_file.close()
+            return output
+
+        return _NUMPY_NDARRAY_FROM_VERSIONS[how](what)
+
+    def AddNumpyNDArrayRepresentation(
+        name: str,
+        /,
+        *,
+        ToVersion: Callable[[array_t], tuple[int, str, str]] = None,
+        FromVersion: Callable[[str], array_t] = None,
+    ) -> None:
+        """"""
+        global _NUMPY_NDARRAY_TO_VERSIONS, _NUMPY_NDARRAY_FROM_VERSIONS
+
+        if name in (NUMPY, NUMPY_COMPRESSED):
             raise ValueError(
-                f'{name}: Invalid keyword-only arguments "ToVersion" and/or "FromVersion". '
-                f"Actual={ToVersion}/{FromVersion}. Expected=Both non-None."
+                f"{NUMPY}, {NUMPY_COMPRESSED}: Reserved representation names"
             )
-        _NUMPY_NDARRAY_TO_VERSIONS[name] = ToVersion
-        _NUMPY_NDARRAY_FROM_VERSIONS[name] = FromVersion
-
-
-def RemoveNumpyNDArrayRepresentation(name: str, /) -> None:
-    """"""
-    global _NUMPY_NDARRAY_TO_VERSIONS, _NUMPY_NDARRAY_FROM_VERSIONS
-
-    if name in (_NUMPY_PLAIN_VERSION, _NUMPY_COMPRESSED_VERSION):
-        raise ValueError(
-            f"{_NUMPY_PLAIN_VERSION}, {_NUMPY_COMPRESSED_VERSION}: Default representations cannot be removed"
-        )
-
-    del _NUMPY_NDARRAY_TO_VERSIONS[name]
-    del _NUMPY_NDARRAY_FROM_VERSIONS[name]
-    if name == _BLOSC_VERSION:
-        del _NUMPY_NDARRAY_FROM_VERSIONS[_BLOSC_BYTES_VERSION]
 
+        if name == BLOSC:
+            if blsc is None:
+                raise ModuleNotFoundError('Module "blosc" not installed or unfoundable')
+            _NUMPY_NDARRAY_TO_VERSIONS[BLOSC] = _BloscVersion
+            _NUMPY_NDARRAY_FROM_VERSIONS[BLOSC] = _FromBloscVersion
+            _NUMPY_NDARRAY_FROM_VERSIONS[BLOSC_BYTES] = _FromBloscBytesVersion
+        elif name == PCA_B_STREAM:
+            if pcst is None:
+                raise ModuleNotFoundError(
+                    'Module "pca_b_stream" not installed or unfoundable'
+                )
+            _NUMPY_NDARRAY_TO_VERSIONS[PCA_B_STREAM] = _PCABStreamVersion
+            _NUMPY_NDARRAY_FROM_VERSIONS[PCA_B_STREAM] = _FromPCABStreamVersion
+        else:
+            if (ToVersion is None) or (FromVersion is None):
+                raise ValueError(
+                    f'{name}: Invalid keyword-only arguments "ToVersion" and/or "FromVersion". '
+                    f"Actual={ToVersion}/{FromVersion}. Expected=Both non-None."
+                )
+            _NUMPY_NDARRAY_TO_VERSIONS[name] = ToVersion
+            _NUMPY_NDARRAY_FROM_VERSIONS[name] = FromVersion
+
+    def RemoveNumpyNDArrayRepresentation(name: str, /) -> None:
+        """"""
+        global _NUMPY_NDARRAY_TO_VERSIONS, _NUMPY_NDARRAY_FROM_VERSIONS
 
-def _BloscVersion(array: array_t, /) -> tuple[str, str] | None:
-    """"""
-    # Do not compare packed instances of an array since blsc.pack_array(array) !=_{can be} blsc.pack_array(array)
-    packed = blsc.pack_array(array)
-    if isinstance(packed, bytes):
-        packed = packed.decode(encoding="iso-8859-1")
-        how = _BLOSC_BYTES_VERSION
-    else:
-        how = _BLOSC_VERSION
-
-    return how, packed
-
-
-def _FromBloscVersion(blosc: str, /) -> array_t:
-    """"""
-    return blsc.unpack_array(blosc)
-
-
-def _FromBloscBytesVersion(blosc: str, /) -> array_t:
-    """"""
-    return blsc.unpack_array(blosc.encode(encoding="iso-8859-1"))
-
-
-def _PCABStreamVersion(array: array_t, /) -> tuple[str, str] | None:
-    """"""
-    if nmpy.issubclass_(
-        array.dtype, (bool, nmpy.bool_, int, nmpy.integer, float, nmpy.floating)
-    ):
-        stream = pcst.PCA2BStream(array).decode(encoding="iso-8859-1")
-        return _PCA_B_STREAM_VERSION, stream
-
-    return None
-
+        if name in (NUMPY, NUMPY_COMPRESSED):
+            raise ValueError(
+                f"{NUMPY}, {NUMPY_COMPRESSED}: Default representations cannot be removed"
+            )
 
-def _FromPCABStreamVersion(pca_b_stream: str, /) -> array_t:
-    """"""
-    return pcst.BStream2PCA(pca_b_stream.encode(encoding="iso-8859-1"))
+        del _NUMPY_NDARRAY_TO_VERSIONS[name]
+        del _NUMPY_NDARRAY_FROM_VERSIONS[name]
+        if name == BLOSC:
+            del _NUMPY_NDARRAY_FROM_VERSIONS[BLOSC_BYTES]
+
+    def _BloscVersion(array: array_t, /) -> tuple[str, str] | None:
+        """"""
+        # Do not compare packed instances of an array since blsc.pack_array(array) !=_{can be} blsc.pack_array(array)
+        packed = blsc.pack_array(array)
+        if isinstance(packed, bytes):
+            packed = packed.decode(encoding="iso-8859-1")
+            how = BLOSC_BYTES
+        else:
+            how = BLOSC
+
+        return how, packed
+
+    def _FromBloscVersion(blosc: str, /) -> array_t:
+        """"""
+        return blsc.unpack_array(blosc)
+
+    def _FromBloscBytesVersion(blosc: str, /) -> array_t:
+        """"""
+        return blsc.unpack_array(blosc.encode(encoding="iso-8859-1"))
+
+    def _PCABStreamVersion(array: array_t, /) -> tuple[str, str] | None:
+        """"""
+        if nmpy.issubclass_(
+            array.dtype, (bool, nmpy.bool_, int, nmpy.integer, float, nmpy.floating)
+        ):
+            stream = pcst.PCA2BStream(array).decode(encoding="iso-8859-1")
+            return PCA_B_STREAM, stream
+
+        return None
+
+    def _FromPCABStreamVersion(pca_b_stream: str, /) -> array_t:
+        """"""
+        return pcst.BStream2PCA(pca_b_stream.encode(encoding="iso-8859-1"))
```

### Comparing `json-any-2023.4/json_any/extension/type.py` & `json-any-2023.5/json_any/extension/type.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,43 +32,43 @@
 import dataclasses as dtcl
 import importlib as imlb
 import sys as sstm
 from types import GenericAlias
 from typing import Any, Callable, Union, get_origin
 
 from json_any.catalog.type import enum_t
+from json_any.constant import MODULE_TYPE_SEPARATOR
 
 builders_h = dict[str, Callable[[Any], Any]]
 description_h = tuple[str, Any]
 descriptors_h = dict[str, Callable[[Any], Any]]
 
 
-_MODULE_SEPARATOR = ":"  # Must be a character forbidden in any (qualified) name
-
-
 class unfound_t:
     pass
 
 
-def FullyQualifiedType(instance_or_type: Union[Any, type], /) -> str:
+def QualifiedType(instance_or_type: Union[Any, type], /) -> str:
     """"""
     # TODO: Explain why an enum_t instance must not be processed by TypeOfInstance.
     if (type(instance_or_type) is type) or issubclass(instance_or_type, enum_t):
         type_ = instance_or_type
     else:
         type_ = TypeOfInstance(instance_or_type)
 
-    return f"{type_.__module__}{_MODULE_SEPARATOR}{type_.__name__}"
+    return f"{type_.__module__}{MODULE_TYPE_SEPARATOR}{type_.__name__}"
 
 
 def TypeFromJsonType(
     json_type: str, /, *, prefix: str = "", should_continue_on_error: bool = False
 ) -> type:
     """"""
-    module, type_ = json_type[prefix.__len__() :].split(_MODULE_SEPARATOR, maxsplit=1)
+    module, type_ = json_type[prefix.__len__() :].split(
+        MODULE_TYPE_SEPARATOR, maxsplit=1
+    )
     error = None
 
     imported = sstm.modules.get(module, None)
     if imported is None:
         # Do not put instead of "None" in "get" above since it will then be evaluated
         # all the time, I suppose.
         try:
```

### Comparing `json-any-2023.4/json_any/json_to_object.py` & `json-any-2023.5/json_any/json_to_object.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,36 +32,35 @@
 import dataclasses as dtcl
 import json
 import pathlib as pthl
 from typing import Any
 
 from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs
 from json_any.catalog.type import (
-    array_t,
+    BUILTIN_BYTES_CONTAINERS_NAMES,
+    BUILTIN_CONTAINERS_NAMES,
+    JSON_TYPE,
+    JSON_TYPE_NUMPY_SCALAR,
+    JSON_TYPE_PREFIX_PATHLIB,
+    ContainerWithName,
     date_t,
     date_time_t,
     enum_t,
-    figure_t,
     io_bytes_t,
     named_tuple_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
 from json_any.constant import (
     CUSTOM_PREFIX,
     DATACLASS_PREFIX,
-    JSON_TYPE,
-    JSON_TYPE_NUMPY_SCALAR,
-    JSON_TYPE_PREFIX_NETWORKX,
-    JSON_TYPE_PREFIX_PANDAS,
-    JSON_TYPE_PREFIX_PATHLIB,
-    JSON_TYPE_PREFIX_SCIPY,
+    MODULE_TYPE_SEPARATOR,
     NEW_FROM_JSON_DESCRIPTION,
     STANDARD_PREFIX,
     UNHANDLED_PREFIX,
 )
 from json_any.extension.numpy import AsNumpyArray
 from json_any.extension.type import (
     TypeFromJsonType,
@@ -152,18 +151,20 @@
                     name = field.name
                     for_init[name] = as_dict[name]
             output = output_t(**for_init)
             # Despite initial values being passed above, all the fields are reset here to their values at JSONing time,
             # again in case things happen in init or post_init.
             for key, value in as_dict.items():
                 setattr(output, key, value)
-    elif json_type in (bytes.__name__, bytearray.__name__):
+    elif json_type in BUILTIN_BYTES_CONTAINERS_NAMES:
+        output_t = ContainerWithName(json_type)
         output = instance.encode(encoding="iso-8859-1")
-        if json_type == bytearray.__name__:
-            output = bytearray(output)
+        if type(output) is not output_t:
+            # In practice, this is only for bytearray since bytes are already bytes.
+            output = output_t(output)
     elif json_type == complex.__name__:
         output = complex(*instance)
     elif json_type == slice.__name__:
         output = slice(*instance)
     elif json_type == JSON_TYPE[uuid_t]:
         output = uuid_t(int=instance)
     elif json_type == JSON_TYPE[date_t]:
@@ -173,38 +174,39 @@
     elif json_type == JSON_TYPE[py_array_t]:
         as_list, typecode = instance
         output = py_array_t(typecode)
         output.fromlist(as_list)
     elif json_type == JSON_TYPE[io_bytes_t]:
         output = io_bytes_t(instance.encode(encoding="iso-8859-1"))
     elif json_type.startswith(JSON_TYPE_PREFIX_PATHLIB):
-        path_type = json_type[JSON_TYPE_PREFIX_PATHLIB.__len__() :]
-        output_t = getattr(pthl, path_type)
+        type_name = json_type[JSON_TYPE_PREFIX_PATHLIB.__len__() :]
+        output_t = getattr(pthl, type_name)
         output = output_t(instance)
-    elif json_type == JSON_TYPE[array_t]:
+    elif TypeIsInModule(json_type, sprs):
+        type_name = TypeNameOf(json_type)
+        output_t = getattr(sprs, type_name)
+        output = output_t(AsNumpyArray(*instance))
+    elif (json_type != JSON_TYPE_NUMPY_SCALAR) and TypeIsInModule(json_type, nmpy):
         output = AsNumpyArray(*instance)
-    elif json_type.startswith(JSON_TYPE_PREFIX_PANDAS):
-        type_name, as_dict = _ObjectFromUnJSONed(
+    elif TypeIsInModule(json_type, pnds):
+        type_name = TypeNameOf(json_type)
+        as_dict = _ObjectFromUnJSONed(
             instance,
             builders=builders,
             should_continue_on_error=should_continue_on_error,
         )
         output_t = getattr(pnds, type_name)
         output = output_t(as_dict)
-    elif json_type.startswith(JSON_TYPE_PREFIX_SCIPY):
-        sparse_type = json_type[JSON_TYPE_PREFIX_SCIPY.__len__() :]
-        output_t = getattr(sprs, sparse_type)
-        output = output_t(AsNumpyArray(*instance))
     elif json_type == JSON_TYPE_NUMPY_SCALAR:
         dtype, value = instance
         if isinstance(value, list):
             output = nmpy.dtype(dtype).type(complex(*value))
         else:
             output = nmpy.dtype(dtype).type(value)
-    elif json_type == JSON_TYPE[figure_t]:
+    elif TypeIsInModule(json_type, pypl):
         fake_file = io_bytes_t(instance.encode(encoding="iso-8859-1"))
         image = pypl.imread(fake_file)
         fake_file.close()
         output, axes = pypl.subplots()
         axes.set_axis_off()
         axes.matshow(image)
     elif json_type == JSON_TYPE[date_time_t]:
@@ -262,47 +264,41 @@
             output = output_t._make(
                 _ObjectFromUnJSONed(
                     instance,
                     builders=builders,
                     should_continue_on_error=should_continue_on_error,
                 )
             )
-    elif json_type in (frozenset.__name__, list.__name__, set.__name__, tuple.__name__):
+    elif json_type in BUILTIN_CONTAINERS_NAMES:
         iterator = (
             _ObjectFromUnJSONed(
                 _elm,
                 builders=builders,
                 should_continue_on_error=should_continue_on_error,
             )
             for _elm in instance
         )
-        if json_type == frozenset.__name__:
-            output = frozenset(iterator)
-        elif json_type == list.__name__:
-            output = list(iterator)
-        elif json_type == set.__name__:
-            output = set(iterator)
-        else:
-            output = tuple(iterator)
+        output_t = ContainerWithName(json_type)
+        output = output_t(iterator)
     elif json_type == dict.__name__:
         output = {
             _ObjectFromUnJSONed(
                 json.loads(_key),
                 builders=builders,
                 should_continue_on_error=should_continue_on_error,
             ): _ObjectFromUnJSONed(
                 _vle,
                 builders=builders,
                 should_continue_on_error=should_continue_on_error,
             )
             for _key, _vle in instance.items()
         }
-    elif json_type.startswith(JSON_TYPE_PREFIX_NETWORKX):
-        graph_type = json_type[JSON_TYPE_PREFIX_NETWORKX.__len__() :]
-        output_t = getattr(grph, graph_type)
+    elif TypeIsInModule(json_type, grph):
+        type_name = TypeNameOf(json_type)
+        output_t = getattr(grph, type_name)
 
         edges_w_attributes = _ObjectFromUnJSONed(
             instance,
             builders=builders,
             should_continue_on_error=should_continue_on_error,
         )
         attributes = {}
@@ -316,10 +312,23 @@
             create_using=output_t,
             multigraph_input=output_t in (grph.MultiGraph, grph.MultiDiGraph),
         )
         grph.set_node_attributes(output, attributes)
     elif json_type.startswith(STANDARD_PREFIX):
         output = instance
     else:
-        raise ValueError(f"{json_type}: Invalid JSON type.")
+        raise ValueError(f"{json_type}: Invalid JSON type or error while unJSONing.")
 
     return output
+
+
+def TypeIsInModule(json_type: str, module: Any, /) -> bool:
+    """"""
+    module_name = module.__name__
+    return json_type.startswith(module_name) and (
+        json_type[module_name.__len__()] in (".", MODULE_TYPE_SEPARATOR)
+    )
+
+
+def TypeNameOf(json_type: str, /) -> str:
+    """"""
+    return json_type[(json_type.rindex(MODULE_TYPE_SEPARATOR) + 1) :]
```

### Comparing `json-any-2023.4/json_any/object_to_json.py` & `json-any-2023.5/json_any/object_to_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,52 +29,55 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import json
 from typing import Any, Sequence
 
-from json_any.catalog.module import grph, nmpy
+from json_any.catalog.module import grph
 from json_any.catalog.type import (
-    NX_GRAPH_CLASSES,
-    SPARSE_ARRAY_CLASSES,
-    array_t,
-    data_frame_t,
+    BUILTIN_BYTES_CONTAINERS,
+    BUILTIN_CONTAINERS,
+    JSON_TYPE,
+    JSON_TYPE_NUMPY_SCALAR,
+    JSON_TYPE_PREFIX_PATHLIB,
+    MATPLOTLIB_CLASSES,
+    NETWORKX_CLASSES,
+    NUMPY_ARRAY_CLASSES,
+    PANDAS_CLASSES,
+    SCIPY_ARRAY_CLASSES,
     date_t,
     date_time_t,
     enum_t,
-    figure_t,
     io_bytes_t,
     named_tuple_t,
     path_t,
     py_array_t,
-    series_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
 from json_any.constant import (
     CUSTOM_PREFIX,
     DATACLASS_PREFIX,
     DESCRIPTION_FOR_JSON,
-    JSON_TYPE,
-    JSON_TYPE_NUMPY_SCALAR,
-    JSON_TYPE_PREFIX_NETWORKX,
-    JSON_TYPE_PREFIX_PATHLIB,
-    JSON_TYPE_PREFIX_SCIPY,
     JSONING_ERROR_MARKER,
     STANDARD_PREFIX,
     UNHANDLED_PREFIX,
 )
-from json_any.extension.numpy import AsMostConciseRepresentation
+from json_any.extension.numpy import (
+    AsMostConciseRepresentation,
+    AsScalarRepresentation,
+    IsNumpyScalar,
+)
 from json_any.extension.type import (
-    FullyQualifiedType,
     IsFullyDataclassBased,
     IsNamedTuple,
+    QualifiedType,
     TypeOfInstance,
     description_h,
     descriptors_h,
 )
 
 _HISTORY_INDENTATION = "    "
 
@@ -100,39 +103,40 @@
     /,
     *,
     highest_level_call: bool = False,
     descriptors: descriptors_h = None,
 ) -> description_h:
     """"""
     instance_type = TypeOfInstance(instance)
-    fully_qualified = FullyQualifiedType(instance_type)
+    json_type = JSON_TYPE.get(instance_type, None)
+    qualified_type = QualifiedType(instance_type)
 
     if descriptors is None:
         descriptors = {}
-    if fully_qualified in descriptors:
-        DescriptionForJSON = descriptors[fully_qualified]
+    if qualified_type in descriptors:
+        DescriptionForJSON = descriptors[qualified_type]
     elif highest_level_call and ("" in descriptors):
-        # Empty key "" is equivalent to FullyQualifiedType(instance) when instance is
+        # Empty key "" is equivalent to QualifiedType(instance) when instance is
         # the object passed to "JsonStringOf". It allows to avoid to have to call
-        # FullyQualifiedType in the first place.
+        # QualifiedType in the first place.
         DescriptionForJSON = descriptors[""]
     else:
         DescriptionForJSON = getattr(instance_type, DESCRIPTION_FOR_JSON, None)
     if DescriptionForJSON is not None:
-        json_type = f"{CUSTOM_PREFIX}{fully_qualified}"
+        json_type = f"{CUSTOM_PREFIX}{qualified_type}"
         history.append(history_level + json_type)
         jsonable = _JsonableVersionOf(
             DescriptionForJSON(instance),
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
     elif dtcl.is_dataclass(instance):
         if IsFullyDataclassBased(instance_type):
-            json_type = f"{DATACLASS_PREFIX}{fully_qualified}"
+            json_type = f"{DATACLASS_PREFIX}{qualified_type}"
             # Do not use dtcl.asdict(instance) since it recurses into dataclass
             # instances which, if they extend a "container" class like list or dict,
             # might lose information.
             description = {
                 _fld.name: getattr(instance, _fld.name)
                 for _fld in dtcl.fields(instance)
             }
@@ -140,153 +144,133 @@
             jsonable = _JsonableVersionOf(
                 description,
                 history,
                 history_level + _HISTORY_INDENTATION,
                 descriptors=descriptors,
             )
         else:
-            json_type = f"{UNHANDLED_PREFIX}{DATACLASS_PREFIX}{fully_qualified}"
+            json_type = f"{UNHANDLED_PREFIX}{DATACLASS_PREFIX}{qualified_type}"
             jsonable = None
             history.append(
                 f"{history_level}{JSONING_ERROR_MARKER}"
                 f"{instance_type.__name__}: Dataclass with inheritance "
                 f'without a "{DESCRIPTION_FOR_JSON}" method. Using None.'
             )
-    # Must be the first type to be tested (see un-findable modules above).
-    elif instance_type in (bytes, bytearray):
+    elif instance_type in BUILTIN_BYTES_CONTAINERS:
         # bytes.hex was initially used in place of bytes.decode.
         json_type = instance_type.__name__
         jsonable = instance.decode(encoding="iso-8859-1")
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is complex:
         json_type = complex.__name__
         jsonable = (instance.real, instance.imag)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is slice:
         json_type = slice.__name__
         jsonable = (instance.start, instance.stop, instance.step)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is uuid_t:
-        json_type, jsonable = JSON_TYPE[uuid_t], instance.int
+        jsonable = instance.int
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is date_t:
-        json_type = JSON_TYPE[date_t]
         jsonable = (instance.year, instance.month, instance.day)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is time_delta_t:
-        json_type = JSON_TYPE[time_delta_t]
         jsonable = (instance.days, instance.seconds, instance.microseconds)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is py_array_t:
-        json_type = JSON_TYPE[py_array_t]
         jsonable = (instance.tolist(), instance.typecode)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is io_bytes_t:
         # Buffer is assumed to be open (i.e. no instance.closed check).
-        json_type = JSON_TYPE[io_bytes_t]
         jsonable = instance.getvalue().decode(encoding="iso-8859-1")
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif issubclass(instance_type, path_t):
         json_type = f"{JSON_TYPE_PREFIX_PATHLIB}{instance_type.__name__}"
         jsonable = str(instance)
         history.append(f"{history_level}{json_type}:{jsonable}")
-    elif instance_type is array_t:
-        json_type, jsonable = JSON_TYPE[array_t], AsMostConciseRepresentation(instance)
+    elif instance_type in SCIPY_ARRAY_CLASSES:
+        jsonable = AsMostConciseRepresentation(instance.toarray())
+        history.append(f"{history_level}{json_type}:{jsonable}")
+    elif instance_type in NUMPY_ARRAY_CLASSES:
+        jsonable = AsMostConciseRepresentation(instance)
         history.append(f"{history_level}{json_type}:{jsonable}")
-    elif instance_type in (data_frame_t, series_t):
-        json_type, jsonable = JSON_TYPE[instance_type], _JsonableVersionOf(
-            (instance_type.__name__, instance.to_dict()),
+    elif instance_type in PANDAS_CLASSES:
+        jsonable = _JsonableVersionOf(
+            instance.to_dict(),
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
         history.append(f"{history_level}{json_type}:{jsonable}")
-    elif instance_type in SPARSE_ARRAY_CLASSES:
-        json_type = f"{JSON_TYPE_PREFIX_SCIPY}{instance_type.__name__}"
-        jsonable = AsMostConciseRepresentation(instance.toarray())
-        history.append(f"{history_level}{json_type}:{jsonable}")
-    elif nmpy.issubclass_(instance_type, (nmpy.bool_, nmpy.number, nmpy.character)):
+    elif IsNumpyScalar(instance_type):
         json_type = JSON_TYPE_NUMPY_SCALAR
-        if nmpy.issubclass_(instance_type, nmpy.bool_):
-            value = bool(instance)
-        elif nmpy.issubclass_(instance_type, nmpy.integer):
-            value = int(instance)
-        elif nmpy.issubclass_(instance_type, nmpy.floating):
-            value = float(instance)
-        elif nmpy.issubclass_(instance_type, complex):
-            # Use list (instead of tuple) since tuples seem to be unJSONed as list, so...
-            value = [float(nmpy.real(instance)), float(nmpy.imag(instance))]
-        else:
-            value = str(instance)
-        jsonable = (instance.dtype.char, value)
+        representation = AsScalarRepresentation(instance, instance_type)
+        jsonable = (instance.dtype.char, representation)
         history.append(f"{history_level}{json_type}:{jsonable}")
-    elif instance_type is figure_t:
+    elif instance_type in MATPLOTLIB_CLASSES:
         fake_file = io_bytes_t()
         instance.canvas.draw()
         instance.savefig(
             fake_file,
             bbox_inches="tight",
             pad_inches=0.0,
             transparent=True,
             dpi=200.0,
             format="png",
         )
-        json_type = JSON_TYPE[figure_t]
         jsonable = fake_file.getvalue().decode(encoding="iso-8859-1")
         fake_file.close()
         history.append(history_level + json_type)
     elif instance_type is date_time_t:
-        json_type = JSON_TYPE[date_time_t]
         history.append(history_level + json_type)
         jsonable = _JsonableVersionOf(
             (instance.date(), instance.timetz()),
             history,
             history_level + _HISTORY_INDENTATION,
         )
     elif instance_type is time_t:
-        json_type = JSON_TYPE[time_t]
         history.append(history_level + json_type)
         jsonable = (
             instance.hour,
             instance.minute,
             instance.second,
             instance.microsecond,
             _JsonableVersionOf(
                 instance.tzinfo, history, history_level + _HISTORY_INDENTATION
             ),
             instance.fold,
         )
     elif instance_type is time_zone_t:
-        json_type = JSON_TYPE[time_zone_t]
         history.append(history_level + json_type)
         jsonable = _JsonableVersionOf(
             (instance.utcoffset(None), instance.tzname(None)),
             history,
             history_level + _HISTORY_INDENTATION,
         )
     elif issubclass(instance_type, enum_t):
-        json_type = f"{JSON_TYPE[enum_t]}{fully_qualified}"
+        json_type = f"{JSON_TYPE[enum_t]}{qualified_type}"
         history.append(history_level + json_type)
         jsonable = _JsonableVersionOf(
             instance.value,
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
     elif IsNamedTuple(instance):
-        json_type = f"{JSON_TYPE[named_tuple_t]}{fully_qualified}"
+        json_type = f"{JSON_TYPE[named_tuple_t]}{qualified_type}"
         as_tuple = tuple(instance)
         history.append(f"{history_level}{json_type}[{as_tuple.__len__()}]")
         jsonable = _JsonableVersionOf(
             as_tuple,
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
-    elif instance_type in (frozenset, list, set, tuple):
+    elif instance_type in BUILTIN_CONTAINERS:
         json_type = instance_type.__name__
         history.append(f"{history_level}{json_type}[{instance.__len__()}]")
         jsonable = [
             _JsonableVersionOf(
                 _elm,
                 history,
                 history_level + _HISTORY_INDENTATION,
@@ -310,22 +294,21 @@
                 _vle,
                 history,
                 history_level + _HISTORY_INDENTATION,
                 descriptors=descriptors,
             )
             for _key, _vle in instance.items()
         }
-    elif instance_type in NX_GRAPH_CLASSES:
+    elif instance_type in NETWORKX_CLASSES:
         edges = grph.to_dict_of_dicts(instance)
         # /!\ Node attributes are added to the edges dictionary! This must be taken into account when deJSONing. Note
         # that several attempts to avoid this have been made, including one relying on repr(node), which is based on
         # hash(node). Since the hash function gives different results across Python sessions, this could not work.
         for node, attributes in instance.nodes(data=True):
             edges[node] = (attributes, edges[node])
-        json_type = f"{JSON_TYPE_PREFIX_NETWORKX}{instance_type.__name__}"
         history.append(history_level + json_type)
         jsonable = _JsonableVersionOf(
             edges,
             history,
             history_level + _HISTORY_INDENTATION,
             descriptors=descriptors,
         )
```

### Comparing `json-any-2023.4/json_any/version.py` & `json-any-2023.5/json_any/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.4"
+__version__ = "2023.5"
```

### Comparing `json-any-2023.4/json_any.egg-info/PKG-INFO` & `json-any-2023.5/json_any.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.4
+Version: 2023.5
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2023.4/setup.py` & `json-any-2023.5/setup.py`

 * *Files identical despite different names*

