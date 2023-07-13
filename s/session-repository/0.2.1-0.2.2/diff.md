# Comparing `tmp/session-repository-0.2.1.tar.gz` & `tmp/session-repository-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.1.tar", last modified: Fri Jul  7 14:13:19 2023, max compression
+gzip compressed data, was "session-repository-0.2.2.tar", last modified: Thu Jul 13 16:21:21 2023, max compression
```

## Comparing `session-repository-0.2.1.tar` & `session-repository-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.163034 session-repository-0.2.1/
--rw-rw-rw-   0        0        0      599 2023-07-07 14:13:19.159901 session-repository-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.079191 session-repository-0.2.1/session_repository/
--rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.1/session_repository/core.py
--rw-rw-rw-   0        0        0      487 2023-06-29 16:01:04.000000 session-repository-0.2.1/session_repository/enum.py
--rw-rw-rw-   0        0        0     8007 2023-07-07 08:14:17.000000 session-repository-0.2.1/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:13:19.146421 session-repository-0.2.1/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-07 14:13:18.000000 session-repository-0.2.1/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 14:13:19.164098 session-repository-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-07 14:12:50.000000 session-repository-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:21:21.433837 session-repository-0.2.2/
+-rw-rw-rw-   0        0        0      599 2023-07-13 16:21:21.431836 session-repository-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 16:21:21.405204 session-repository-0.2.2/session_repository/
+-rw-rw-rw-   0        0        0     9287 2023-07-07 14:12:40.000000 session-repository-0.2.2/session_repository/core.py
+-rw-rw-rw-   0        0        0      549 2023-07-13 16:15:21.000000 session-repository-0.2.2/session_repository/enum.py
+-rw-rw-rw-   0        0        0     8591 2023-07-13 16:20:14.000000 session-repository-0.2.2/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:21:21.428831 session-repository-0.2.2/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-13 16:21:21.000000 session-repository-0.2.2/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-13 16:21:21.000000 session-repository-0.2.2/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:21:21.000000 session-repository-0.2.2/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-13 16:21:21.000000 session-repository-0.2.2/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-13 16:21:21.000000 session-repository-0.2.2/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 16:21:21.434838 session-repository-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-13 16:20:53.000000 session-repository-0.2.2/setup.py
```

### Comparing `session-repository-0.2.1/PKG-INFO` & `session-repository-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.1
+Version: 0.2.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.1/session_repository/core.py` & `session-repository-0.2.2/session_repository/core.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.1/session_repository/utils.py` & `session-repository-0.2.2/session_repository/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Iterable,
     List,
     Tuple,
     Union,
 )
 
 # SQLALCHEMY
-from sqlalchemy import and_, asc, desc, tuple_
+from sqlalchemy import and_, asc, desc, tuple_, func
 from sqlalchemy.orm import (
     Query,
     InstrumentedAttribute,
     noload,
 )
 from sqlalchemy.sql.elements import Null
 
@@ -155,14 +155,24 @@
                     case Operators.DIFFERENT:
                         conditions.append(key != v)
                     case Operators.LIKE:
                         if not isinstance(v, Null):
                             conditions.append(key.like(v))
                         else:
                             conditions.append(key == v)
+                    case Operators.LIKE_LOWER:
+                        if not isinstance(v, Null):
+                            conditions.append(func.lower(key).like(v.lower()))
+                        else:
+                            conditions.append(func.lower(key) == v.lower())
+                    case Operators.LIKE_UPPER:
+                        if not isinstance(v, Null):
+                            conditions.append(func.upper(key).like(v.upper()))
+                        else:
+                            conditions.append(func.upper(key) == v.upper())
                     case Operators.NOT_LIKE:
                         if not isinstance(v, Null):
                             conditions.append(~key.like(v))
                         else:
                             conditions.append(key != v)
                     case Operators.ILIKE:
                         if not isinstance(v, Null):
```

### Comparing `session-repository-0.2.1/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.2/session_repository.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.1
+Version: 0.2.2
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.1/setup.py` & `session-repository-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.1"
+version = "0.2.2"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
     ],
```

