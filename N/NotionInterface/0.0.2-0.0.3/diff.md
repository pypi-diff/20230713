# Comparing `tmp/NotionInterface-0.0.2.tar.gz` & `tmp/NotionInterface-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionInterface-0.0.2.tar", last modified: Thu Jul 13 17:54:11 2023, max compression
+gzip compressed data, was "NotionInterface-0.0.3.tar", last modified: Thu Jul 13 19:14:02 2023, max compression
```

## Comparing `NotionInterface-0.0.2.tar` & `NotionInterface-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 17:54:11.364767 NotionInterface-0.0.2/
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 17:54:11.363594 NotionInterface-0.0.2/NotionInterface/
--rw-r--r--   0 lukapedra   (501) staff       (20)      119 2023-07-13 17:26:00.000000 NotionInterface-0.0.2/NotionInterface/__init__.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-06-20 12:23:58.000000 NotionInterface-0.0.2/NotionInterface/constants.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     5286 2023-07-06 18:36:15.000000 NotionInterface-0.0.2/NotionInterface/notion_database.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-06 18:36:53.000000 NotionInterface-0.0.2/NotionInterface/notion_database_types.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-06-20 12:23:58.000000 NotionInterface-0.0.2/NotionInterface/notion_header.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      657 2023-07-13 17:23:08.000000 NotionInterface-0.0.2/NotionInterface/notion_page.py
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 17:54:11.364446 NotionInterface-0.0.2/NotionInterface.egg-info/
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 17:54:11.000000 NotionInterface-0.0.2/NotionInterface.egg-info/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-13 17:54:11.000000 NotionInterface-0.0.2/NotionInterface.egg-info/SOURCES.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-13 17:54:11.000000 NotionInterface-0.0.2/NotionInterface.egg-info/dependency_links.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-13 17:54:11.000000 NotionInterface-0.0.2/NotionInterface.egg-info/requires.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-13 17:54:11.000000 NotionInterface-0.0.2/NotionInterface.egg-info/top_level.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 17:54:11.364634 NotionInterface-0.0.2/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.2/README.md
--rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-13 17:54:11.364809 NotionInterface-0.0.2/setup.cfg
--rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-13 17:53:45.000000 NotionInterface-0.0.2/setup.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.521296 NotionInterface-0.0.3/
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.520114 NotionInterface-0.0.3/NotionInterface/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-13 19:13:24.000000 NotionInterface-0.0.3/NotionInterface/__init__.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/NotionInterface/constants.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     5286 2023-07-06 18:36:15.000000 NotionInterface-0.0.3/NotionInterface/notion_database.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-06 18:36:53.000000 NotionInterface-0.0.3/NotionInterface/notion_database_types.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/NotionInterface/notion_header.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-13 19:07:31.000000 NotionInterface-0.0.3/NotionInterface/notion_page.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.520995 NotionInterface-0.0.3/NotionInterface.egg-info/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/requires.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/top_level.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 19:14:02.521176 NotionInterface-0.0.3/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/README.md
+-rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-13 19:14:02.521340 NotionInterface-0.0.3/setup.cfg
+-rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-13 19:13:40.000000 NotionInterface-0.0.3/setup.py
```

### Comparing `NotionInterface-0.0.2/NotionInterface/notion_database.py` & `NotionInterface-0.0.3/NotionInterface/notion_database.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.2/NotionInterface/notion_database_types.py` & `NotionInterface-0.0.3/NotionInterface/notion_database_types.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.2/NotionInterface/notion_page.py` & `NotionInterface-0.0.3/NotionInterface/notion_page.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-import notion_header as notion_header
+import NotionInterface.notion_header as notion_header
 
 
 class NotionPage:
 	page_id:str
 	key:str
 	dbList = []
 	def __init__(self, page_id:str, notion_key:str):
```

### Comparing `NotionInterface-0.0.2/NotionInterface.egg-info/PKG-INFO` & `NotionInterface-0.0.3/NotionInterface.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionInterface
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Notion db interface for Python
 Home-page: UNKNOWN
 Author: LukaPedra (Lucca Rocha)
 Author-email: <lucca.v.rocha@gmail.com>
 License: UNKNOWN
 Keywords: python,Notion,Database,page,Block,pandas
 Platform: UNKNOWN
```

### Comparing `NotionInterface-0.0.2/PKG-INFO` & `NotionInterface-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionInterface
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Notion db interface for Python
 Home-page: UNKNOWN
 Author: LukaPedra (Lucca Rocha)
 Author-email: <lucca.v.rocha@gmail.com>
 License: UNKNOWN
 Keywords: python,Notion,Database,page,Block,pandas
 Platform: UNKNOWN
```

### Comparing `NotionInterface-0.0.2/setup.py` & `NotionInterface-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A simple Notion db interface for Python'
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 # Setting up
 setup(
```

