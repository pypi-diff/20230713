# Comparing `tmp/fastapi-tusd-0.0.1.tar.gz` & `tmp/fastapi-tusd-0.100.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-7p16mldd/fastapi-tusd-0.0.1.tar", last modified: Tue Jul 11 16:00:54 2023, max compression
+gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-ii5lsn6e/fastapi-tusd-0.100.0.tar", last modified: Thu Jul 13 03:51:04 2023, max compression
```

## Comparing `fastapi-tusd-0.0.1.tar` & `fastapi-tusd-0.100.0.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/examples/app_tusd.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/src/fastapi_tusd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/src/fastapi_tusd/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/src/fastapi_tusd/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-11 16:00:43.000000 fastapi-tusd-0.0.1/src/fastapi_tusd/tusd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:00:53.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 16:00:54.000000 fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/examples/app_tusd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/tusd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/top_level.txt
```

### Comparing `fastapi-tusd-0.0.1/.github/workflows/publish.yml` & `fastapi-tusd-0.100.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/.gitignore` & `fastapi-tusd-0.100.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/LICENSE` & `fastapi-tusd-0.100.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/PKG-INFO` & `fastapi-tusd-0.100.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.0.1
+Version: 0.100.0
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
 Keywords: fastapi_tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: format
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # FastAPI Server for Tus Protocol
 
 A file upload server of the tus resumable upload protocol is implemented on FastAPI framework.  
 
@@ -42,17 +43,19 @@
 app = FastAPI()
 
 app.include_router(TusRouter(store_dir="./files", prefix="/files"))
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
-### Example with Tus Client
+### Examples
 
-A simple example with web client using `uppy` to support for `Tus` protocol, under the `example/` folder
+There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
+
+Enter the `example/` folder, run(`pip install uvicorn` if no `uvicorn`!)
 
 ```sh
 uvicorn app_tusd:app --reload
 ```
 
 Then visit `https://127.0.0.1:8000/upload.thml`
```

### Comparing `fastapi-tusd-0.0.1/README.md` & `fastapi-tusd-0.100.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 app = FastAPI()
 
 app.include_router(TusRouter(store_dir="./files", prefix="/files"))
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
-### Example with Tus Client
+### Examples
 
-A simple example with web client using `uppy` to support for `Tus` protocol, under the `example/` folder
+There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
+
+Enter the `example/` folder, run(`pip install uvicorn` if no `uvicorn`!)
 
 ```sh
 uvicorn app_tusd:app --reload
 ```
 
 Then visit `https://127.0.0.1:8000/upload.thml`
```

### Comparing `fastapi-tusd-0.0.1/example.py` & `fastapi-tusd-0.100.0/example.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/examples/app_tusd.py` & `fastapi-tusd-0.100.0/examples/app_tusd.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/setup.cfg` & `fastapi-tusd-0.100.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 include_package_data = True
 packages = find_namespace:
 python_requires = >=3.7
 package_dir = 
 	=src
 zip_safe = False
 install_requires = 
-	fastapi>=0.98
+	fastapi>=0.100.0
 	filelock
-	uvicorn
 
 [options.packages.find]
 where = src
 exclude = tests*
 
 [options.package_data]
 * = *.txt, *.rst
@@ -46,12 +45,14 @@
 
 [options.extras_require]
 test = 
 	pytest>=3
 	pytest-cov
 format = 
 	black
+dev = 
+	uvicorn
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fastapi-tusd-0.0.1/src/fastapi_tusd/filestore.py` & `fastapi-tusd-0.100.0/src/fastapi_tusd/filestore.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/src/fastapi_tusd/tusd.py` & `fastapi-tusd-0.100.0/src/fastapi_tusd/tusd.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.0.1/src/fastapi_tusd.egg-info/PKG-INFO` & `fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.0.1
+Version: 0.100.0
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
 Keywords: fastapi_tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: format
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # FastAPI Server for Tus Protocol
 
 A file upload server of the tus resumable upload protocol is implemented on FastAPI framework.  
 
@@ -42,17 +43,19 @@
 app = FastAPI()
 
 app.include_router(TusRouter(store_dir="./files", prefix="/files"))
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
-### Example with Tus Client
+### Examples
 
-A simple example with web client using `uppy` to support for `Tus` protocol, under the `example/` folder
+There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
+
+Enter the `example/` folder, run(`pip install uvicorn` if no `uvicorn`!)
 
 ```sh
 uvicorn app_tusd:app --reload
 ```
 
 Then visit `https://127.0.0.1:8000/upload.thml`
```

