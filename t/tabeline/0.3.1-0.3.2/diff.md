# Comparing `tmp/tabeline-0.3.1.tar.gz` & `tmp/tabeline-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabeline-0.3.1.tar", max compression
+gzip compressed data, was "tabeline-0.3.2.tar", max compression
```

## Comparing `tabeline-0.3.1.tar` & `tabeline-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-06-28 10:08:20.880692 tabeline-0.3.1/LICENSE
--rw-r--r--   0        0        0     1708 2023-04-26 09:54:10.670471 tabeline-0.3.1/README.md
--rw-r--r--   0        0        0     2304 2023-07-09 12:51:46.917779 tabeline-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-09 12:51:14.429760 tabeline-0.3.1/src/tabeline/__init__.py
--rw-r--r--   0        0        0     1419 2023-06-28 15:53:44.753714 tabeline-0.3.1/src/tabeline/_concatenate.py
--rw-r--r--   0        0        0    22789 2023-07-09 12:51:15.537760 tabeline-0.3.1/src/tabeline/_data_frame.py
--rw-r--r--   0        0        0      365 2023-04-21 01:31:22.563413 tabeline-0.3.1/src/tabeline/_dummy.py
--rw-r--r--   0        0        0      139 2023-06-28 15:38:00.904206 tabeline-0.3.1/src/tabeline/_expression/__init__.py
--rw-r--r--   0        0        0     3671 2023-07-09 12:51:15.537760 tabeline-0.3.1/src/tabeline/_expression/_functions.py
--rw-r--r--   0        0        0     4071 2023-06-27 13:13:14.028287 tabeline-0.3.1/src/tabeline/_expression/_parser.py
--rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.3.1/src/tabeline/_expression/_substitute.py
--rw-r--r--   0        0        0     3744 2023-06-29 12:57:02.032034 tabeline-0.3.1/src/tabeline/_expression/_to_polars.py
--rw-r--r--   0        0        0     2788 2023-06-27 13:13:17.724278 tabeline-0.3.1/src/tabeline/_expression/ast.py
--rw-r--r--   0        0        0      796 2023-07-04 16:11:44.006619 tabeline-0.3.1/src/tabeline/_validation.py
--rw-r--r--   0        0        0     3965 2023-07-04 15:02:57.136441 tabeline-0.3.1/src/tabeline/exceptions.py
--rw-r--r--   0        0        0      381 2023-04-21 01:31:22.559414 tabeline-0.3.1/src/tabeline/testing.py
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 tabeline-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-28 10:08:20.880692 tabeline-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1708 2023-04-26 09:54:10.670471 tabeline-0.3.2/README.md
+-rw-r--r--   0        0        0     2384 2023-07-13 00:49:12.827405 tabeline-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-07-10 12:10:48.897883 tabeline-0.3.2/src/tabeline/__init__.py
+-rw-r--r--   0        0        0     2783 2023-07-13 00:38:00.198492 tabeline-0.3.2/src/tabeline/_array.py
+-rw-r--r--   0        0        0     1419 2023-06-28 15:53:44.753714 tabeline-0.3.2/src/tabeline/_concatenate.py
+-rw-r--r--   0        0        0    24814 2023-07-13 00:19:47.013511 tabeline-0.3.2/src/tabeline/_data_frame.py
+-rw-r--r--   0        0        0      365 2023-04-21 01:31:22.563413 tabeline-0.3.2/src/tabeline/_dummy.py
+-rw-r--r--   0        0        0      139 2023-06-28 15:38:00.904206 tabeline-0.3.2/src/tabeline/_expression/__init__.py
+-rw-r--r--   0        0        0     3713 2023-07-10 12:10:48.897883 tabeline-0.3.2/src/tabeline/_expression/_functions.py
+-rw-r--r--   0        0        0     4071 2023-06-27 13:13:14.028287 tabeline-0.3.2/src/tabeline/_expression/_parser.py
+-rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.3.2/src/tabeline/_expression/_substitute.py
+-rw-r--r--   0        0        0     3744 2023-06-29 12:57:02.032034 tabeline-0.3.2/src/tabeline/_expression/_to_polars.py
+-rw-r--r--   0        0        0     2788 2023-06-27 13:13:17.724278 tabeline-0.3.2/src/tabeline/_expression/ast.py
+-rw-r--r--   0        0        0     1720 2023-07-10 12:10:48.897883 tabeline-0.3.2/src/tabeline/_record.py
+-rw-r--r--   0        0        0      796 2023-07-11 00:43:59.656830 tabeline-0.3.2/src/tabeline/_validation.py
+-rw-r--r--   0        0        0     3965 2023-07-04 15:02:57.136441 tabeline-0.3.2/src/tabeline/exceptions.py
+-rw-r--r--   0        0        0      381 2023-04-21 01:31:22.559414 tabeline-0.3.2/src/tabeline/testing.py
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 tabeline-0.3.2/PKG-INFO
```

### Comparing `tabeline-0.3.1/LICENSE` & `tabeline-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/README.md` & `tabeline-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/pyproject.toml` & `tabeline-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tabeline"
-version = "0.3.1"
+version = "0.3.2"
 description = "A data frame and data grammar library"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://tabeline.drhagen.com"
 repository = "https://github.com/drhagen/tabeline"
 keywords = ["dataframe", "datatable", "datagrammar", "dplyr"]
@@ -93,15 +93,16 @@
     "C4", # flake8-comprehensions
     "PIE", # flake8-pie
     "PT", # flake8-pytest-style
     "PTH", # flake8-use-pathlib
     "ERA", # flake8-eradicate
 ]
 # F821: undefined-name; Parsita triggers this, but code coverage will catch it
-extend-ignore = ["F821"]
+# B905: zip-without-explicit-strict; strict not available in Python 3.9
+extend-ignore = ["F821", "B905"]
 
 [tool.ruff.per-file-ignores]
 # F401: unused-import; Allow unused imports in __init__.py files
 "__init__.py" = ["F401"]
 
 [tool.ruff.isort]
 extra-standard-library = ["typing_extensions"]
```

### Comparing `tabeline-0.3.1/src/tabeline/_concatenate.py` & `tabeline-0.3.2/src/tabeline/_concatenate.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/_data_frame.py` & `tabeline-0.3.2/src/tabeline/_data_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 __all__ = ["DataFrame"]
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Literal, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, Sequence, Union, overload
 
 import polars as pl
 
+from ._array import Array
 from ._dummy import dummy_frame, dummy_name
 from ._expression import substitute, to_polars
 from ._expression.ast import Expression
+from ._record import Record
 from ._validation import assert_legal_columns, missing
 from .exceptions import (
     GroupColumnError,
     HasGroupsError,
     IndexOutOfRangeError,
     NoGroupsError,
     NonexistentColumnError,
@@ -24,23 +26,36 @@
 error = object()
 
 if TYPE_CHECKING:
     import pandas as pd
 
 
 class DataFrame:
+    @overload
+    def __init__(self, **columns: list[bool] | list[int] | list[float] | list[str]):
+        pass
+
+    @overload
+    def __init__(
+        self,
+        polars_df: pl.DataFrame,
+        group_levels: tuple[tuple[str, ...], ...] = (),
+        height: Optional[int] = None,
+    ):
+        pass
+
     def __init__(
         self,
         polars_df: pl.DataFrame = missing,
         group_levels: tuple[tuple[str, ...], ...] = (),
         height: Optional[int] = None,
         /,
-        **columns,
+        **columns: list[bool] | list[int] | list[float] | list[str],
     ):
-        self.groups: tuple[tuple[str, ...], ...]
+        self.group_levels: tuple[tuple[str, ...], ...]
 
         if polars_df is missing:
             self._df = pl.DataFrame(columns)
             self.group_levels = ()
             self.height = self._df.height  # With no columns, height is assumed to be 0
         elif len(columns) == 0:
             self._df = polars_df
@@ -69,20 +84,26 @@
         return tuple(self._df.columns)
 
     @property
     def group_names(self) -> tuple[str, ...]:
         return tuple(names for level in self.group_levels for names in level)
 
     @staticmethod
-    def from_dict(columns: dict[str, list[Any]], /) -> DataFrame:
-        df = pl.DataFrame(columns)
+    def from_dict(columns: dict[str, Sequence[Any]], /) -> DataFrame:
+        df = pl.from_dict(columns)
         return DataFrame(df)
 
+    def to_dict(self) -> dict[str, Array]:
+        if len(self.group_levels) != 0:
+            raise HasGroupsError()
+
+        return {name: Array(series) for name, series in self._df.to_dict().items()}
+
     @staticmethod
-    def from_pandas(df: pd.DataFrame) -> DataFrame:
+    def from_pandas(df: pd.DataFrame, /) -> DataFrame:
         if df.shape[1] == 0:
             # Polars does not understand columnless data frames
             return DataFrame.columnless(height=df.shape[0])
 
         return DataFrame(pl.from_pandas(df))
 
     def to_pandas(self) -> pd.DataFrame:
@@ -95,29 +116,29 @@
         if self.width == 0:
             # Polars does not understand columnless data frames
             return pd.DataFrame(np.empty((self.height, 0)))
 
         return self._df.to_pandas()
 
     @staticmethod
-    def from_polars(df: pl.DataFrame) -> DataFrame:
+    def from_polars(df: pl.DataFrame, /) -> DataFrame:
         return DataFrame(df)
 
     def to_polars(self) -> pl.DataFrame:
         if len(self.group_levels) != 0:
             raise HasGroupsError()
 
         return self._df
 
     @staticmethod
-    def read_csv(path: Path) -> DataFrame:
+    def read_csv(path: Path, /) -> DataFrame:
         df = pl.read_csv(str(path))
         return DataFrame(df)
 
-    def write_csv(self, path: Path) -> None:
+    def write_csv(self, path: Path, /) -> None:
         if len(self.group_levels) != 0:
             raise HasGroupsError()
 
         self._df.write_csv(str(path))
 
     def slice0(self, indexes: list[int], /) -> DataFrame:
         # Negative indexes are not supported by Polars, so they are not
@@ -577,14 +598,51 @@
             .drop(["_index1", "_index2"])
             .collect()
         )
         return DataFrame(
             joined_df,
         )
 
+    @overload
+    def __getitem__(self, key: tuple[int, str]) -> bool | int | float | str:
+        pass
+
+    @overload
+    def __getitem__(self, key: tuple[int, Sequence[str]]) -> Record:
+        pass
+
+    @overload
+    def __getitem__(self, key: tuple[Sequence[int] | Sequence[bool], str]) -> Array:
+        pass
+
+    @overload
+    def __getitem__(self, key: tuple[Sequence[int] | Sequence[bool], Sequence[str]]) -> DataFrame:
+        pass
+
+    def __getitem__(
+        self, key: tuple[int | Sequence[int] | Sequence[bool], str | Sequence[str]]
+    ) -> DataFrame | Array | Record | bool | int | float | str:
+        row_index, column_index = key
+
+        if isinstance(column_index, str):
+            if isinstance(row_index, int):
+                return self._df.item(row_index, column_index)
+            else:
+                return Array(self._df[column_index][row_index])
+        elif column_index == slice(None):
+            if isinstance(row_index, int):
+                return Record(self._df.row(row_index, named=True))
+            else:
+                return DataFrame(self._df[row_index, :], (), len(row_index))
+        else:
+            if isinstance(row_index, int):
+                return Record(self._df.select(column_index).row(row_index, named=True))
+            else:
+                return DataFrame(self._df[row_index, column_index], (), len(row_index))
+
     def __eq__(self, other):
         if isinstance(other, DataFrame):
             if self.group_levels != other.group_levels:
                 return False
 
             if self.width == 0:
                 # Polars does not understand columnless data frames
```

### Comparing `tabeline-0.3.1/src/tabeline/_expression/_functions.py` & `tabeline-0.3.2/src/tabeline/_expression/_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,16 @@
     Function("max", lambda x: x.max()),
     Function("min", lambda x: x.min()),
     Function("sum", lambda x: x.sum()),
     Function("mean", lambda x: x.mean()),
     Function("median", lambda x: x.median()),
     Function(
         "quantile",
-        lambda x, quantile: x.quantile(pl.select(quantile)[0, 0], interpolation="linear"),
-    ),
+        lambda x, quantile: x.quantile(pl.select(quantile).item(), interpolation="linear"),
+    ),  # https://stackoverflow.com/a/71721580/
     Function(
         "trapz", lambda x, y: 0.5 * ((x - x.shift()) * (y + y.shift())).sum()
     ),  # https://github.com/pola-rs/polars/issues/3043
     Function(
         "interp",
         lambda x, xp, fp: pl.apply(
             exprs=[x, xp, fp],
```

### Comparing `tabeline-0.3.1/src/tabeline/_expression/_parser.py` & `tabeline-0.3.2/src/tabeline/_expression/_parser.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/_expression/_substitute.py` & `tabeline-0.3.2/src/tabeline/_expression/_substitute.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/_expression/_to_polars.py` & `tabeline-0.3.2/src/tabeline/_expression/_to_polars.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/_expression/ast.py` & `tabeline-0.3.2/src/tabeline/_expression/ast.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/_validation.py` & `tabeline-0.3.2/src/tabeline/_validation.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/src/tabeline/exceptions.py` & `tabeline-0.3.2/src/tabeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.1/PKG-INFO` & `tabeline-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabeline
-Version: 0.3.1
+Version: 0.3.2
 Summary: A data frame and data grammar library
 Home-page: https://github.com/drhagen/tabeline
 License: MIT
 Keywords: dataframe,datatable,datagrammar,dplyr
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.9,<4.0
```

