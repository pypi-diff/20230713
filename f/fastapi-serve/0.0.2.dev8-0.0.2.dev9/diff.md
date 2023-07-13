# Comparing `tmp/fastapi-serve-0.0.2.dev8.tar.gz` & `tmp/fastapi-serve-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.2.dev8.tar", last modified: Wed Jul 12 15:30:22 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.2.dev9.tar", last modified: Wed Jul 12 15:32:10 2023, max compression
```

## Comparing `fastapi-serve-0.0.2.dev8.tar` & `fastapi-serve-0.0.2.dev9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:30:22.291889 fastapi-serve-0.0.2.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:30:22.291889 fastapi-serve-0.0.2.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:30:22.287889 fastapi-serve-0.0.2.dev8/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 15:30:21.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:30:22.291889 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:30:22.291889 fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:30:22.287889 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:30:22.000000 fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:30:22.291889 fastapi-serve-0.0.2.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 15:30:17.000000 fastapi-serve-0.0.2.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:32:10.000000 fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:32:10.518041 fastapi-serve-0.0.2.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 15:32:04.000000 fastapi-serve-0.0.2.dev9/setup.py
```

### Comparing `fastapi-serve-0.0.2.dev8/LICENSE` & `fastapi-serve-0.0.2.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/PKG-INFO` & `fastapi-serve-0.0.2.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev9 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev8/README.md` & `fastapi-serve-0.0.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/__main__.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve/helper.py` & `fastapi-serve-0.0.2.dev9/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev8 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.2.dev9 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
```

### Comparing `fastapi-serve-0.0.2.dev8/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.2.dev9/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.2.dev8/setup.py` & `fastapi-serve-0.0.2.dev9/setup.py`

 * *Files identical despite different names*

