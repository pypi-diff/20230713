# Comparing `tmp/mediacatch-s2t-1.0.0.tar.gz` & `tmp/mediacatch-s2t-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mediacatch-s2t/mediacatch-s2t/dist/.tmp-30zie4fq/mediacatch-s2t-1.0.0.tar", last modified: Mon Jun  5 06:41:01 2023, max compression
+gzip compressed data, was "/home/runner/work/mediacatch-s2t/mediacatch-s2t/dist/.tmp-6iu0ib9q/mediacatch-s2t-1.0.1.tar", last modified: Thu Jul 13 12:49:04 2023, max compression
```

## Comparing `mediacatch-s2t-1.0.0.tar` & `mediacatch-s2t-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:41:01.000000 mediacatch-s2t-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-05 06:40:49.000000 mediacatch-s2t-1.0.0/tests/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:49:04.000000 mediacatch-s2t-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/tests/test_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-13 12:48:48.000000 mediacatch-s2t-1.0.1/tests/test_uploader.py
```

### Comparing `mediacatch-s2t-1.0.0/LICENSE` & `mediacatch-s2t-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/PKG-INFO` & `mediacatch-s2t-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 1.0.0
+Version: 1.0.1
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MediaCatch Speech-To-Text Uploader
 
-![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/github-action.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
+![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/lint-and-pytest.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
 
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
```

### Comparing `mediacatch-s2t-1.0.0/README.md` & `mediacatch-s2t-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MediaCatch Speech-To-Text Uploader
 
-![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/github-action.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
+![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/lint-and-pytest.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
 
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
```

### Comparing `mediacatch-s2t-1.0.0/pyproject.toml` & `mediacatch-s2t-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mediacatch-s2t"
-version = '1.0.0'
+version = '1.0.1'
 description = "Upload a media file and get the transcription link."
 readme = "README.md"
 authors = [{ name = "MediaCatch", email = "support@mediacatch.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t/__init__.py` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """MediaCatch speech-to-text file uploader.
 
 """
 
 # Version of the mc-s2t-mediacatch_s2t
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 import os
 
 URL: str = os.environ.get('MEDIACATCH_URL', 'https://s2t.mediacatch.io')
 SINGLE_UPLOAD_ENDPOINT: str = os.environ.get(
     'MEDIACATCH_PRESIGN_ENDPOINT',
     '/presigned-post-url')
```

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t/__main__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t/helper.py` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,12 +52,12 @@
 
     current_version = read_installed_version()
     latest_version = check_latest_version()
     if latest_version and current_version < latest_version:
         subprocess.run([
             "python", "-m",
             "pip", "install",
-            f"{_PACKAGE_NAME}", "-U", "--quite"
+            f"{_PACKAGE_NAME}", "-U", "--quiet"
         ])
         set_last_update()
         return True
     return False
```

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t/uploader.py` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t/uploader.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 1.0.0
+Version: 1.0.1
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -187,15 +187,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # MediaCatch Speech-To-Text Uploader
 
-![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/github-action.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
+![github test](https://github.com/mediacatch/mediacatch-s2t/actions/workflows/lint-and-pytest.yml/badge.svg) [![codecov](https://codecov.io/gh/mediacatch/mediacatch-s2t/branch/main/graph/badge.svg?token=ZQ36ZRJ2ZU)](https://codecov.io/gh/mediacatch/mediacatch-s2t)
 
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
```

### Comparing `mediacatch-s2t-1.0.0/src/mediacatch_s2t.egg-info/SOURCES.txt` & `mediacatch-s2t-1.0.1/src/mediacatch_s2t.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/tests/test_helper.py` & `mediacatch-s2t-1.0.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/tests/test_multipart_upload.py` & `mediacatch-s2t-1.0.1/tests/test_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-1.0.0/tests/test_uploader.py` & `mediacatch-s2t-1.0.1/tests/test_uploader.py`

 * *Files identical despite different names*

