# Comparing `tmp/XoxoDay-0.0.26.tar.gz` & `tmp/XoxoDay-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.26.tar", last modified: Mon Jul  3 10:12:20 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.27.tar", last modified: Wed Jul 12 14:05:32 2023, max compression
```

## Comparing `XoxoDay-0.0.26.tar` & `XoxoDay-0.0.27.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:12:20.452435 XoxoDay-0.0.26/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.26/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-03 10:12:20.452293 XoxoDay-0.0.26/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.26/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:12:20.448890 XoxoDay-0.0.26/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-03 10:12:08.000000 XoxoDay-0.0.26/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.26/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:12:20.450318 XoxoDay-0.0.26/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.26/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.26/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      909 2023-07-03 10:12:08.000000 XoxoDay-0.0.26/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.26/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:12:20.451950 XoxoDay-0.0.26/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.26/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.26/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.26/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3003 2023-06-23 22:30:27.000000 XoxoDay-0.0.26/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.26/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.26/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-03 10:12:20.449772 XoxoDay-0.0.26/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-03 10:12:20.000000 XoxoDay-0.0.26/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-07-03 10:12:20.000000 XoxoDay-0.0.26/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-03 10:12:20.000000 XoxoDay-0.0.26/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-03 10:12:20.000000 XoxoDay-0.0.26/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-03 10:12:20.000000 XoxoDay-0.0.26/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-03 10:12:20.452480 XoxoDay-0.0.26/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-03 10:12:12.000000 XoxoDay-0.0.26/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-12 14:05:32.586716 XoxoDay-0.0.27/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.27/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-12 14:05:32.586577 XoxoDay-0.0.27/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.27/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-12 14:05:32.583560 XoxoDay-0.0.27/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-07-12 14:05:20.000000 XoxoDay-0.0.27/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.27/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-12 14:05:32.584602 XoxoDay-0.0.27/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.27/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      790 2023-07-12 11:07:51.000000 XoxoDay-0.0.27/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.27/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-12 14:05:32.586258 XoxoDay-0.0.27/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.27/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.27/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.27/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1892 2023-07-12 13:59:14.000000 XoxoDay-0.0.27/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.27/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.27/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-07-12 14:05:32.584363 XoxoDay-0.0.27/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-07-12 14:05:32.000000 XoxoDay-0.0.27/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      483 2023-07-12 14:05:32.000000 XoxoDay-0.0.27/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-07-12 14:05:32.000000 XoxoDay-0.0.27/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-07-12 14:05:32.000000 XoxoDay-0.0.27/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-07-12 14:05:32.000000 XoxoDay-0.0.27/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-07-12 14:05:32.586768 XoxoDay-0.0.27/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-07-12 14:05:15.000000 XoxoDay-0.0.27/setup.py
```

### Comparing `XoxoDay-0.0.26/LICENSE` & `XoxoDay-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.26/PKG-INFO` & `XoxoDay-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.26
+Version: 0.0.27
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.26/README.md` & `XoxoDay-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.26/XoxoDay/exception.py` & `XoxoDay-0.0.27/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.26/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.27/XoxoDay/helper/token.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 import sys
-import sqlite3 as lite
 
 from XoxoDay.exception import XoxoDayException
+from XoxoDay.serializer import Serializer
 
-sql_path = f'{os.path.dirname(os.path.abspath(__file__))}/xoxo.sqlite'
+ROOT_DIR = os.path.split(os.environ['VIRTUAL_ENV'])[0] if 'VIRTUAL_ENV' in os.environ else sys.path[1]
 
-ROOT_DIR = sys.path[1]
+file_path = f'{ROOT_DIR}/xoxo_json'
 
 
-def initialize_sql_lite():
+def get_token():
     try:
-        with lite.connect(sql_path) as sqlite:
-            cursor = sqlite.cursor()
-            query = "CREATE TABLE IF NOT EXISTS jwt (token json)"
-            cursor.execute(query)
-            sqlite.commit()
+        with open(file_path, "r") as file:
+            token_dict = file.read()
+            if token_dict is not None:
+                token_dict = Serializer.loads(token_dict[0])
+            file.close()
+            return token_dict
     except Exception as e:
         raise XoxoDayException(e)
 
 
-def get_cookie():
-    f = open(f'{ROOT_DIR}/xoxo_cookie', "r")
-    cookie = f.read()
-    f.close()
-    return cookie
+def update_token(token):
+    try:
+        with open(file_path, "wb") as file:
+            file.write(Serializer.dumps(token))
+            file.close()
+    except Exception as e:
+        raise XoxoDayException(e)
```

### Comparing `XoxoDay-0.0.26/XoxoDay/service/http_service.py` & `XoxoDay-0.0.27/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.26/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.27/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.26/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.27/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.26
+Version: 0.0.27
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.26/setup.py` & `XoxoDay-0.0.27/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.26",
+    version="0.0.27",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

