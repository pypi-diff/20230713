# Comparing `tmp/pggm_datalab_utils-2.8.tar.gz` & `tmp/pggm_datalab_utils-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pggm_datalab_utils-2.8.tar", max compression
+gzip compressed data, was "pggm_datalab_utils-2.9.tar", max compression
```

## Comparing `pggm_datalab_utils-2.8.tar` & `pggm_datalab_utils-2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2022-12-29 10:50:03.268897 pggm_datalab_utils-2.8/LICENSE
--rw-r--r--   0        0        0     9528 2023-01-26 15:13:56.886735 pggm_datalab_utils-2.8/pggm_datalab_utils/db.py
--rw-r--r--   0        0        0     1154 2022-12-29 10:50:12.887987 pggm_datalab_utils-2.8/pggm_datalab_utils/flatten.py
--rw-r--r--   0        0        0      549 2023-01-26 15:14:46.280342 pggm_datalab_utils-2.8/pyproject.toml
--rw-r--r--   0        0        0      729 2022-12-29 10:54:25.272611 pggm_datalab_utils-2.8/readme.md
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pggm_datalab_utils-2.8/setup.py
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 pggm_datalab_utils-2.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-12-29 10:50:03.268897 pggm_datalab_utils-2.9/LICENSE
+-rw-r--r--   0        0        0     9540 2023-02-24 09:32:22.591669 pggm_datalab_utils-2.9/pggm_datalab_utils/db.py
+-rw-r--r--   0        0        0     1160 2023-02-24 09:32:03.972422 pggm_datalab_utils-2.9/pggm_datalab_utils/flatten.py
+-rw-r--r--   0        0        0      549 2023-02-24 09:43:00.807938 pggm_datalab_utils-2.9/pyproject.toml
+-rw-r--r--   0        0        0      729 2022-12-29 10:54:25.272611 pggm_datalab_utils-2.9/readme.md
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pggm_datalab_utils-2.9/setup.py
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 pggm_datalab_utils-2.9/PKG-INFO
```

### Comparing `pggm_datalab_utils-2.8/LICENSE` & `pggm_datalab_utils-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pggm_datalab_utils-2.8/pggm_datalab_utils/db.py` & `pggm_datalab_utils-2.9/pggm_datalab_utils/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from contextlib import contextmanager
 from datetime import datetime
 import json
 import logging
 import os
 import pyodbc
 import sqlite3
-from typing import Optional, Iterator, Any, Union, Hashable
+from typing import Dict, List, Optional, Iterator, Any, Union, Hashable
 
 Connection = Union[pyodbc.Connection, sqlite3.Connection]  # Todo: unify in own interface to get autocomplete
 Cursor = Union[pyodbc.Cursor, sqlite3.Cursor]
-Record = dict[str, Any]
-RecordList = list[Record]
+Record = Dict[str, Any]
+RecordList = List[Record]
 
 
 def get_db_connection(server: str, database: str) -> Connection:
     """
     Initiate pyodbc connection to a SQL Server database. This function is intended to be suitable for cloud development:
     in the cloud you use environment variables to log in under a certain username and password, whereas locally you
     simply log in using your AAD credentials.
```

### Comparing `pggm_datalab_utils-2.8/pggm_datalab_utils/flatten.py` & `pggm_datalab_utils-2.9/pggm_datalab_utils/flatten.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Iterable, Any
+from typing import Iterable, Any, List
 from itertools import accumulate
 import operator as op
 
 
-def flatten(it: Iterable[Iterable[Any]]) -> list[Any]:
+def flatten(it: Iterable[Iterable[Any]]) -> List[Any]:
     """
     Flatten a list of lists, or any kind of nested iterable, into a single list.
     """
     return [x for item in it for x in item]
 
 
-def flatten_with_mapping(it: Iterable[list[Any]]) -> (list[Any], list[int]):
+def flatten_with_mapping(it: Iterable[List[Any]]) -> (List[Any], List[int]):
     """
     Flatten a list of lists, or any kind of nested iterable, into a single list, additionally returning the lengths
     of each of the items, allowing you to restore the original list of lists using `unflatten`.
     We test that `unflatten(*flatten_with_mapping(x)) == x` and vice versa.
     """
     return [x for item in it for x in item], [len(item) for item in it]
 
 
-def unflatten(flattened: list[Any], mapping: list[int]) -> list[list[Any]]:
+def unflatten(flattened: List[Any], mapping: List[int]) -> List[List[Any]]:
     """
     Unflatten a list, breaking it into sublists of length indicated by `mapping`.
     We test that `unflatten(*flatten_with_mapping(x)) == x` and vice versa.
     """
     indices = list(accumulate(mapping, op.add))
     return [flattened[start:end] for start, end in zip([0] + indices[:-1], indices)]
```

### Comparing `pggm_datalab_utils-2.8/pyproject.toml` & `pggm_datalab_utils-2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pggm-datalab-utils"
-version = "2.8"
+version = "2.9"
 description = "Utilities created and used by the Datalab of PGGM"
 authors = ["Rik de Kort <rik.de.kort@pggm.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pggm_datalab_utils"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pggm_datalab_utils-2.8/readme.md` & `pggm_datalab_utils-2.9/readme.md`

 * *Files identical despite different names*

### Comparing `pggm_datalab_utils-2.8/setup.py` & `pggm_datalab_utils-2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyodbc>=4.0.34,<5.0.0']
 
 setup_kwargs = {
     'name': 'pggm-datalab-utils',
-    'version': '2.8',
+    'version': '2.9',
     'description': 'Utilities created and used by the Datalab of PGGM',
     'long_description': "# Datalab utils\nWell-specified utilities from the Datalab of PGGM. Our aim with this package is to provide some tooling to make our lives a bit easier.\nSo far the package contains:\n- Database utilities, allowing you to connect to cloud databases using pyodbc in a standard pattern.\n- Helpers around nested lists (flattening and unflattening).\n- Helpers to make working with lists of dictionaries a bit easier so you don't have to resort to Pandas as fast.\n\n## How to use the database helpers\n```python\nfrom pggm_datalab_utils.db import cursor, query\n\nbbg_id = 'WOW'\n\nwith cursor('pggm-sql-lre-o.database.windows.net', 'lre') as c:\n    data = query(c, 'select sedol, name from portfolio where bbg_id=?', bbg_id)\n```",
     'author': 'Rik de Kort',
     'author_email': 'rik.de.kort@pggm.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pggm_datalab_utils-2.8/PKG-INFO` & `pggm_datalab_utils-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pggm-datalab-utils
-Version: 2.8
+Version: 2.9
 Summary: Utilities created and used by the Datalab of PGGM
 License: MIT
 Author: Rik de Kort
 Author-email: rik.de.kort@pggm.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

