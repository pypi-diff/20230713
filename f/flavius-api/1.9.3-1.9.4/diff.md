# Comparing `tmp/flavius-api-1.9.3.tar.gz` & `tmp/flavius-api-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavius-api-1.9.3.tar", last modified: Thu Feb  3 05:32:42 2022, max compression
+gzip compressed data, was "flavius-api-1.9.4.tar", last modified: Thu Feb  3 05:44:54 2022, max compression
```

## Comparing `flavius-api-1.9.3.tar` & `flavius-api-1.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:32:42.256874 flavius-api-1.9.3/
--rw-r--r--   0 koichiezato   (501) staff       (20)        0 2021-11-05 04:35:55.000000 flavius-api-1.9.3/LICENSE
--rw-r--r--   0 koichiezato   (501) staff       (20)      625 2022-02-03 05:32:42.256930 flavius-api-1.9.3/PKG-INFO
--rw-r--r--   0 koichiezato   (501) staff       (20)       65 2021-11-05 04:35:55.000000 flavius-api-1.9.3/README.md
--rw-r--r--   0 koichiezato   (501) staff       (20)      123 2021-11-05 04:35:55.000000 flavius-api-1.9.3/pyproject.toml
--rw-r--r--   0 koichiezato   (501) staff       (20)      678 2022-02-03 05:32:42.257200 flavius-api-1.9.3/setup.cfg
--rw-r--r--   0 koichiezato   (501) staff       (20)       39 2021-11-05 04:35:55.000000 flavius-api-1.9.3/setup.py
-drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:32:42.254686 flavius-api-1.9.3/src/
-drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:32:42.256147 flavius-api-1.9.3/src/flavius_api/
--rw-r--r--   0 koichiezato   (501) staff       (20)       60 2021-11-05 04:35:55.000000 flavius-api-1.9.3/src/flavius_api/__init__.py
--rw-r--r--   0 koichiezato   (501) staff       (20)    10408 2022-02-03 05:11:20.000000 flavius-api-1.9.3/src/flavius_api/api.py
--rw-r--r--   0 koichiezato   (501) staff       (20)      371 2021-11-05 04:35:55.000000 flavius-api-1.9.3/src/flavius_api/checks.py
--rw-r--r--   0 koichiezato   (501) staff       (20)     5182 2022-02-03 04:34:04.000000 flavius-api-1.9.3/src/flavius_api/conf.py
-drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:32:42.256777 flavius-api-1.9.3/src/flavius_api.egg-info/
--rw-r--r--   0 koichiezato   (501) staff       (20)      625 2022-02-03 05:32:42.000000 flavius-api-1.9.3/src/flavius_api.egg-info/PKG-INFO
--rw-r--r--   0 koichiezato   (501) staff       (20)      346 2022-02-03 05:32:42.000000 flavius-api-1.9.3/src/flavius_api.egg-info/SOURCES.txt
--rw-r--r--   0 koichiezato   (501) staff       (20)        1 2022-02-03 05:32:42.000000 flavius-api-1.9.3/src/flavius_api.egg-info/dependency_links.txt
--rw-r--r--   0 koichiezato   (501) staff       (20)        9 2022-02-03 05:32:42.000000 flavius-api-1.9.3/src/flavius_api.egg-info/requires.txt
--rw-r--r--   0 koichiezato   (501) staff       (20)       12 2022-02-03 05:32:42.000000 flavius-api-1.9.3/src/flavius_api.egg-info/top_level.txt
+drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:44:54.532733 flavius-api-1.9.4/
+-rw-r--r--   0 koichiezato   (501) staff       (20)        0 2021-11-05 04:35:55.000000 flavius-api-1.9.4/LICENSE
+-rw-r--r--   0 koichiezato   (501) staff       (20)      625 2022-02-03 05:44:54.532780 flavius-api-1.9.4/PKG-INFO
+-rw-r--r--   0 koichiezato   (501) staff       (20)       65 2021-11-05 04:35:55.000000 flavius-api-1.9.4/README.md
+-rw-r--r--   0 koichiezato   (501) staff       (20)      123 2021-11-05 04:35:55.000000 flavius-api-1.9.4/pyproject.toml
+-rw-r--r--   0 koichiezato   (501) staff       (20)      678 2022-02-03 05:44:54.533021 flavius-api-1.9.4/setup.cfg
+-rw-r--r--   0 koichiezato   (501) staff       (20)       39 2021-11-05 04:35:55.000000 flavius-api-1.9.4/setup.py
+drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:44:54.530659 flavius-api-1.9.4/src/
+drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:44:54.532020 flavius-api-1.9.4/src/flavius_api/
+-rw-r--r--   0 koichiezato   (501) staff       (20)       60 2021-11-05 04:35:55.000000 flavius-api-1.9.4/src/flavius_api/__init__.py
+-rw-r--r--   0 koichiezato   (501) staff       (20)    10380 2022-02-03 05:41:59.000000 flavius-api-1.9.4/src/flavius_api/api.py
+-rw-r--r--   0 koichiezato   (501) staff       (20)      371 2021-11-05 04:35:55.000000 flavius-api-1.9.4/src/flavius_api/checks.py
+-rw-r--r--   0 koichiezato   (501) staff       (20)     5182 2022-02-03 04:34:04.000000 flavius-api-1.9.4/src/flavius_api/conf.py
+drwxr-xr-x   0 koichiezato   (501) staff       (20)        0 2022-02-03 05:44:54.532647 flavius-api-1.9.4/src/flavius_api.egg-info/
+-rw-r--r--   0 koichiezato   (501) staff       (20)      625 2022-02-03 05:44:54.000000 flavius-api-1.9.4/src/flavius_api.egg-info/PKG-INFO
+-rw-r--r--   0 koichiezato   (501) staff       (20)      346 2022-02-03 05:44:54.000000 flavius-api-1.9.4/src/flavius_api.egg-info/SOURCES.txt
+-rw-r--r--   0 koichiezato   (501) staff       (20)        1 2022-02-03 05:44:54.000000 flavius-api-1.9.4/src/flavius_api.egg-info/dependency_links.txt
+-rw-r--r--   0 koichiezato   (501) staff       (20)        9 2022-02-03 05:44:54.000000 flavius-api-1.9.4/src/flavius_api.egg-info/requires.txt
+-rw-r--r--   0 koichiezato   (501) staff       (20)       12 2022-02-03 05:44:54.000000 flavius-api-1.9.4/src/flavius_api.egg-info/top_level.txt
```

### Comparing `flavius-api-1.9.3/PKG-INFO` & `flavius-api-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavius-api
-Version: 1.9.3
+Version: 1.9.4
 Summary: FlaviusへAPI接続するためのパッケージ
 Home-page: https://github.com/gnsjapan/flavuis_api
 Author: Koichi Ezato
 Author-email: ezato@gnsjapan.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/gnsjapan/flavuis_api/issues
 Platform: UNKNOWN
```

### Comparing `flavius-api-1.9.3/setup.cfg` & `flavius-api-1.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flavius-api
-version = 1.9.3
+version = 1.9.4
 author = Koichi Ezato
 author_email = ezato@gnsjapan.jp
 description = FlaviusへAPI接続するためのパッケージ
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gnsjapan/flavuis_api
 project_urls =
```

### Comparing `flavius-api-1.9.3/src/flavius_api/api.py` & `flavius-api-1.9.4/src/flavius_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,8 +259,8 @@
         super(FlaviusPickupLocationFileUpload, self).__init__(search_url='',
                                                               create_url=conf.FLAVIUS_API_PICKUP_LOCATION_FILE_UPLOAD,
                                                               update_url='',
                                                               delete_url='')
 
     def create(self, query=None):
         with requests.post(self.create_url, files=query, data=query) as response:
-            return json.loads(response.read().decode('utf-8'))
+            return response.json()
```

### Comparing `flavius-api-1.9.3/src/flavius_api/conf.py` & `flavius-api-1.9.4/src/flavius_api/conf.py`

 * *Files identical despite different names*

### Comparing `flavius-api-1.9.3/src/flavius_api.egg-info/PKG-INFO` & `flavius-api-1.9.4/src/flavius_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavius-api
-Version: 1.9.3
+Version: 1.9.4
 Summary: FlaviusへAPI接続するためのパッケージ
 Home-page: https://github.com/gnsjapan/flavuis_api
 Author: Koichi Ezato
 Author-email: ezato@gnsjapan.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/gnsjapan/flavuis_api/issues
 Platform: UNKNOWN
```

