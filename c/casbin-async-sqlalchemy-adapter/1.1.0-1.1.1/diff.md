# Comparing `tmp/casbin_async_sqlalchemy_adapter-1.1.0.tar.gz` & `tmp/casbin_async_sqlalchemy_adapter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.1.0.tar", last modified: Sun May 21 17:35:52 2023, max compression
+gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.1.1.tar", last modified: Thu Jul 13 09:32:36 2023, max compression
```

## Comparing `casbin_async_sqlalchemy_adapter-1.1.0.tar` & `casbin_async_sqlalchemy_adapter-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 17:35:51.000000 casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:35:51.996077 casbin_async_sqlalchemy_adapter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-21 17:35:20.000000 casbin_async_sqlalchemy_adapter-1.1.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/tests/test_adapter.py
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/LICENSE` & `casbin_async_sqlalchemy_adapter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_sqlalchemy_adapter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/README.md` & `casbin_async_sqlalchemy_adapter-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/__init__.py` & `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter/adapter.py` & `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 import warnings
 from contextlib import asynccontextmanager
 
 from casbin import persist
 from sqlalchemy import Column, Integer, String
 from sqlalchemy import or_
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
-from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.future import select
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import declarative_base, sessionmaker
 
 Base = declarative_base()
 
 
 class CasbinRule(Base):
     __tablename__ = "casbin_rule"
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-async-sqlalchemy-adapter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/setup.py` & `casbin_async_sqlalchemy_adapter-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.0/tests/test_adapter.py` & `casbin_async_sqlalchemy_adapter-1.1.1/tests/test_adapter.py`

 * *Files identical despite different names*

