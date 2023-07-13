# Comparing `tmp/session-repository-0.2.4.tar.gz` & `tmp/session-repository-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.4.tar", last modified: Thu Jul 13 16:50:37 2023, max compression
+gzip compressed data, was "session-repository-0.2.5.tar", last modified: Thu Jul 13 16:52:56 2023, max compression
```

## Comparing `session-repository-0.2.4.tar` & `session-repository-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:50:37.476566 session-repository-0.2.4/
--rw-rw-rw-   0        0        0      599 2023-07-13 16:50:37.472952 session-repository-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 16:50:37.434467 session-repository-0.2.4/session_repository/
--rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.4/session_repository/core.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.4/session_repository/enum.py
--rw-rw-rw-   0        0        0     9545 2023-07-13 16:50:01.000000 session-repository-0.2.4/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:50:37.465628 session-repository-0.2.4/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-13 16:50:37.000000 session-repository-0.2.4/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-13 16:50:37.000000 session-repository-0.2.4/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:50:37.000000 session-repository-0.2.4/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 16:50:37.000000 session-repository-0.2.4/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-13 16:50:37.000000 session-repository-0.2.4/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 16:50:37.477568 session-repository-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-13 16:50:18.000000 session-repository-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.484063 session-repository-0.2.5/
+-rw-rw-rw-   0        0        0      599 2023-07-13 16:52:56.480840 session-repository-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.456909 session-repository-0.2.5/session_repository/
+-rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.5/session_repository/core.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.5/session_repository/enum.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.5/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:52:56.476840 session-repository-0.2.5/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-13 16:52:56.000000 session-repository-0.2.5/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:52:56.485065 session-repository-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-13 16:52:37.000000 session-repository-0.2.5/setup.py
```

### Comparing `session-repository-0.2.4/PKG-INFO` & `session-repository-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.4
+Version: 0.2.5
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.4/session_repository/core.py` & `session-repository-0.2.5/session_repository/core.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.4/session_repository/enum.py` & `session-repository-0.2.5/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.4/session_repository/utils.py` & `session-repository-0.2.5/session_repository/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from sqlalchemy import and_, asc, desc, tuple_, func
 from sqlalchemy.orm import (
     Query,
     InstrumentedAttribute,
     noload,
 )
 from sqlalchemy.sql.elements import Null
-from sqlalchemy.sql.expression import escape
 
 # Enum
 from session_repository.enum import Operators
 
 _FilterType = Dict[Union[InstrumentedAttribute, Tuple[InstrumentedAttribute]], Any]
```

### Comparing `session-repository-0.2.4/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.5/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.4
+Version: 0.2.5
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.4/setup.py` & `session-repository-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.4"
+version = "0.2.5"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

