# Comparing `tmp/ormstorm-0.0.2.tar.gz` & `tmp/ormstorm-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormstorm-0.0.2.tar", last modified: Tue Jul 11 17:48:52 2023, max compression
+gzip compressed data, was "ormstorm-0.0.2.1.tar", last modified: Thu Jul 13 14:42:41 2023, max compression
```

## Comparing `ormstorm-0.0.2.tar` & `ormstorm-0.0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/
--rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstorm-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3393 2023-07-11 17:48:52.612443 ormstorm-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.578669 ormstorm-0.0.2/ormstorm/
--rw-rw-rw-   0        0        0     7431 2023-07-11 17:20:56.000000 ormstorm-0.0.2/ormstorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/ormstorm/orm/
--rw-rw-rw-   0        0        0        0 2023-07-10 20:02:40.000000 ormstorm-0.0.2/ormstorm/orm/__init__.py
--rw-rw-rw-   0        0        0     2480 2023-07-11 17:16:41.000000 ormstorm-0.0.2/ormstorm/orm/column.py
--rw-rw-rw-   0        0        0      455 2023-07-10 13:15:35.000000 ormstorm-0.0.2/ormstorm/orm/constants.py
--rw-rw-rw-   0        0        0       48 2023-07-11 13:35:28.000000 ormstorm-0.0.2/ormstorm/orm/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.612443 ormstorm-0.0.2/ormstorm/orm/filters/
--rw-rw-rw-   0        0        0       32 2023-07-11 17:16:41.000000 ormstorm-0.0.2/ormstorm/orm/filters/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-07-11 17:29:00.000000 ormstorm-0.0.2/ormstorm/orm/filters/magic.py
--rw-rw-rw-   0        0        0     2674 2023-07-10 13:26:33.000000 ormstorm-0.0.2/ormstorm/orm/table.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:48:52.594805 ormstorm-0.0.2/ormstorm.egg-info/
--rw-rw-rw-   0        0        0     3393 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 17:48:52.000000 ormstorm-0.0.2/ormstorm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:48:52.612443 ormstorm-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-07-11 17:48:29.000000 ormstorm-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/
+-rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstorm-0.0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3395 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 14:42:41.387877 ormstorm-0.0.2.1/ormstorm/
+-rw-rw-rw-   0        0        0     7495 2023-07-13 14:40:13.000000 ormstorm-0.0.2.1/ormstorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/ormstorm/orm/
+-rw-rw-rw-   0        0        0        0 2023-07-10 20:02:40.000000 ormstorm-0.0.2.1/ormstorm/orm/__init__.py
+-rw-rw-rw-   0        0        0     2480 2023-07-11 17:16:41.000000 ormstorm-0.0.2.1/ormstorm/orm/column.py
+-rw-rw-rw-   0        0        0      455 2023-07-10 13:15:35.000000 ormstorm-0.0.2.1/ormstorm/orm/constants.py
+-rw-rw-rw-   0        0        0       48 2023-07-11 13:35:28.000000 ormstorm-0.0.2.1/ormstorm/orm/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/ormstorm/orm/filters/
+-rw-rw-rw-   0        0        0       32 2023-07-11 17:16:41.000000 ormstorm-0.0.2.1/ormstorm/orm/filters/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-07-11 17:29:00.000000 ormstorm-0.0.2.1/ormstorm/orm/filters/magic.py
+-rw-rw-rw-   0        0        0     2674 2023-07-13 14:10:09.000000 ormstorm-0.0.2.1/ormstorm/orm/table.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/ormstorm.egg-info/
+-rw-rw-rw-   0        0        0     3395 2023-07-13 14:42:41.000000 ormstorm-0.0.2.1/ormstorm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-13 14:42:41.000000 ormstorm-0.0.2.1/ormstorm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:42:41.000000 ormstorm-0.0.2.1/ormstorm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 14:42:41.000000 ormstorm-0.0.2.1/ormstorm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 14:42:41.391351 ormstorm-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-07-13 14:42:17.000000 ormstorm-0.0.2.1/setup.py
```

### Comparing `ormstorm-0.0.2/LICENSE.txt` & `ormstorm-0.0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.2/PKG-INFO` & `ormstorm-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormstorm
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Small library for easy work with databases.
 Author: Molchaliv
 Author-email: molchaliv666@gmail.com
 Keywords: python,orm,database,sql,sqlite3
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ormstorm-0.0.2/ormstorm/__init__.py` & `ormstorm-0.0.2.1/ormstorm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlite3
 
 from .orm.filters import MagicFilter
 from .orm.column import Column, ColumnType
 from .orm.constants import Types
 from .orm.exceptions import SessionExecuteError
 from .orm.table import Table, DynamicTable
+from .utils.dict_factory import dict_factory
 
 from typing import Callable, Union, Type
 
 
 class Typing(object):
 
     """
@@ -134,15 +135,15 @@
                 f"SELECT EXISTS(SELECT * FROM {data.__tablename__})"
             ).fetchone()[-1]
 
         return not not self._database.execute(
             f"SELECT EXISTS(SELECT * FROM {data.parameters['table']} WHERE {data.query})", data.variables
         ).fetchone()[-1]
 
-    def select(self, data: Typing.AnyTable, items: list[Typing.AnyColumn] = None) -> list[tuple]:
+    def select(self, data: Typing.AnyTable, items: list[Typing.AnyColumn] = None) -> list[dict[str, object]]:
 
         """
         Selects certain data from a table that satisfies given conditions.
 
         :param data: Any type of table or magic filter
         :param items: Elements to select
         :return: List of tuples
@@ -152,21 +153,21 @@
             raise SessionExecuteError("The data is not a successor of MagicFilterData or Table!")
 
         select = "*" if not items else ", ".join(
             [f"{item.table}.{item.name}" for item in items]
         )
 
         if isinstance(data, (DynamicTable, Table, type(Table))):
-            return self._database.execute(
+            return dict_factory(self._database.execute(
                 f"SELECT {select} FROM {data.__tablename__}"
-            ).fetchall()
+            ))
 
-        return self._database.execute(
+        return dict_factory(self._database.execute(
             f"SELECT {select} FROM {data.parameters['table']} WHERE {data.query}", data.variables
-        ).fetchall()
+        ))
 
     def count(self, data: Typing.AnyTable) -> int:
 
         """
         Counts the number of rows satisfying given conditions.
 
         :param data: Any type of table or magic filter
```

### Comparing `ormstorm-0.0.2/ormstorm/orm/column.py` & `ormstorm-0.0.2.1/ormstorm/orm/column.py`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.2/ormstorm/orm/filters/magic.py` & `ormstorm-0.0.2.1/ormstorm/orm/filters/magic.py`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.2/ormstorm/orm/table.py` & `ormstorm-0.0.2.1/ormstorm/orm/table.py`

 * *Files identical despite different names*

### Comparing `ormstorm-0.0.2/ormstorm.egg-info/PKG-INFO` & `ormstorm-0.0.2.1/ormstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormstorm
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Small library for easy work with databases.
 Author: Molchaliv
 Author-email: molchaliv666@gmail.com
 Keywords: python,orm,database,sql,sqlite3
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ormstorm-0.0.2/setup.py` & `ormstorm-0.0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.2.1"
 DESCRIPTION = "Small library for easy work with databases."
 
 with open("READ ME.md", mode="r", encoding="utf-8") as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name="ormstorm",
```

