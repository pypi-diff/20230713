# Comparing `tmp/pyresponseio-0.0.1.tar.gz` & `tmp/pyresponseio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresponseio-0.0.1.tar", last modified: Thu Jul 13 00:46:57 2023, max compression
+gzip compressed data, was "pyresponseio-0.0.2.tar", last modified: Thu Jul 13 01:24:46 2023, max compression
```

## Comparing `pyresponseio-0.0.1.tar` & `pyresponseio-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 00:46:57.581975 pyresponseio-0.0.1/
--rw-r--r--   0 ipeluwa    (501) staff       (20)     1076 2023-07-12 22:56:06.000000 pyresponseio-0.0.1/LICENSE
--rw-r--r--   0 ipeluwa    (501) staff       (20)      597 2023-07-13 00:46:57.580838 pyresponseio-0.0.1/PKG-INFO
--rw-r--r--   0 ipeluwa    (501) staff       (20)     5009 2023-07-12 23:54:48.000000 pyresponseio-0.0.1/README.md
-drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 00:46:57.573251 pyresponseio-0.0.1/pyresponse/
--rw-r--r--   0 ipeluwa    (501) staff       (20)        0 2023-07-12 22:59:12.000000 pyresponseio-0.0.1/pyresponse/__init__.py
--rw-r--r--   0 ipeluwa    (501) staff       (20)      260 2023-07-12 23:53:00.000000 pyresponseio-0.0.1/pyresponse/config.py
--rw-r--r--   0 ipeluwa    (501) staff       (20)      799 2023-07-12 23:52:44.000000 pyresponseio-0.0.1/pyresponse/logging.py
--rw-r--r--   0 ipeluwa    (501) staff       (20)     2534 2023-07-13 00:27:55.000000 pyresponseio-0.0.1/pyresponse/response.py
-drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 00:46:57.577943 pyresponseio-0.0.1/pyresponseio.egg-info/
--rw-r--r--   0 ipeluwa    (501) staff       (20)      597 2023-07-13 00:46:57.000000 pyresponseio-0.0.1/pyresponseio.egg-info/PKG-INFO
--rw-r--r--   0 ipeluwa    (501) staff       (20)      294 2023-07-13 00:46:57.000000 pyresponseio-0.0.1/pyresponseio.egg-info/SOURCES.txt
--rw-r--r--   0 ipeluwa    (501) staff       (20)        1 2023-07-13 00:46:57.000000 pyresponseio-0.0.1/pyresponseio.egg-info/dependency_links.txt
--rw-r--r--   0 ipeluwa    (501) staff       (20)       54 2023-07-13 00:46:57.000000 pyresponseio-0.0.1/pyresponseio.egg-info/requires.txt
--rw-r--r--   0 ipeluwa    (501) staff       (20)       11 2023-07-13 00:46:57.000000 pyresponseio-0.0.1/pyresponseio.egg-info/top_level.txt
--rw-r--r--   0 ipeluwa    (501) staff       (20)       38 2023-07-13 00:46:57.582171 pyresponseio-0.0.1/setup.cfg
--rw-r--r--   0 ipeluwa    (501) staff       (20)     1012 2023-07-13 00:44:22.000000 pyresponseio-0.0.1/setup.py
+drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 01:24:46.210207 pyresponseio-0.0.2/
+-rw-r--r--   0 ipeluwa    (501) staff       (20)     1076 2023-07-12 22:56:06.000000 pyresponseio-0.0.2/LICENSE
+-rw-r--r--   0 ipeluwa    (501) staff       (20)      597 2023-07-13 01:24:46.209780 pyresponseio-0.0.2/PKG-INFO
+-rw-r--r--   0 ipeluwa    (501) staff       (20)     5009 2023-07-12 23:54:48.000000 pyresponseio-0.0.2/README.md
+drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 01:24:46.203359 pyresponseio-0.0.2/pyresponse/
+-rw-r--r--   0 ipeluwa    (501) staff       (20)        0 2023-07-12 22:59:12.000000 pyresponseio-0.0.2/pyresponse/__init__.py
+-rw-r--r--   0 ipeluwa    (501) staff       (20)      260 2023-07-12 23:53:00.000000 pyresponseio-0.0.2/pyresponse/config.py
+-rw-r--r--   0 ipeluwa    (501) staff       (20)      799 2023-07-12 23:52:44.000000 pyresponseio-0.0.2/pyresponse/logging.py
+-rw-r--r--   0 ipeluwa    (501) staff       (20)     2524 2023-07-13 01:22:31.000000 pyresponseio-0.0.2/pyresponse/response.py
+drwxr-xr-x   0 ipeluwa    (501) staff       (20)        0 2023-07-13 01:24:46.208927 pyresponseio-0.0.2/pyresponseio.egg-info/
+-rw-r--r--   0 ipeluwa    (501) staff       (20)      597 2023-07-13 01:24:46.000000 pyresponseio-0.0.2/pyresponseio.egg-info/PKG-INFO
+-rw-r--r--   0 ipeluwa    (501) staff       (20)      294 2023-07-13 01:24:46.000000 pyresponseio-0.0.2/pyresponseio.egg-info/SOURCES.txt
+-rw-r--r--   0 ipeluwa    (501) staff       (20)        1 2023-07-13 01:24:46.000000 pyresponseio-0.0.2/pyresponseio.egg-info/dependency_links.txt
+-rw-r--r--   0 ipeluwa    (501) staff       (20)       54 2023-07-13 01:24:46.000000 pyresponseio-0.0.2/pyresponseio.egg-info/requires.txt
+-rw-r--r--   0 ipeluwa    (501) staff       (20)       11 2023-07-13 01:24:46.000000 pyresponseio-0.0.2/pyresponseio.egg-info/top_level.txt
+-rw-r--r--   0 ipeluwa    (501) staff       (20)       38 2023-07-13 01:24:46.210318 pyresponseio-0.0.2/setup.cfg
+-rw-r--r--   0 ipeluwa    (501) staff       (20)     1012 2023-07-13 01:22:46.000000 pyresponseio-0.0.2/setup.py
```

### Comparing `pyresponseio-0.0.1/LICENSE` & `pyresponseio-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyresponseio-0.0.1/PKG-INFO` & `pyresponseio-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresponseio
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for creating success and error responses in Python Projects
 Author: Ibrahim Oluwapeluwa
 Author-email: ipeluwa@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyresponseio-0.0.1/README.md` & `pyresponseio-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyresponseio-0.0.1/pyresponse/logging.py` & `pyresponseio-0.0.2/pyresponse/logging.py`

 * *Files identical despite different names*

### Comparing `pyresponseio-0.0.1/pyresponse/response.py` & `pyresponseio-0.0.2/pyresponse/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 import logging
 from typing import Any
 
 
 class Response:
-    def __init__(self, data: Any, status_code: int):
+    def __init__(self, data: Any, status: int):
         self.data = data
-        self.status_code = status_code
+        self.status_code = status
 
 
 def create_success_response(data=None, message=None, status_code=None, serializer=None, **kwargs):
     """
     Create a success response.
 
     This function generates a success response with the provided data, message,
```

### Comparing `pyresponseio-0.0.1/pyresponseio.egg-info/PKG-INFO` & `pyresponseio-0.0.2/pyresponseio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresponseio
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for creating success and error responses in Python Projects
 Author: Ibrahim Oluwapeluwa
 Author-email: ipeluwa@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyresponseio-0.0.1/setup.py` & `pyresponseio-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from readme_renderer import markdown
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme_content = f.read()
 
 setup(
     name='pyresponseio',
-    version='0.0.1',
+    version='0.0.2',
     description='Package for creating success and error responses in Python Projects',
     long_description=markdown.render(readme_content),
     long_description_content_type='text/markdown',
     author='Ibrahim Oluwapeluwa',
     author_email='ipeluwa@gmail.com',
     packages=find_packages(),
     install_requires=[
```

