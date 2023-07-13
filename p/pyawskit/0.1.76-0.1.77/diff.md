# Comparing `tmp/pyawskit-0.1.76.tar.gz` & `tmp/pyawskit-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.76.tar", last modified: Thu Jul 13 04:39:11 2023, max compression
+gzip compressed data, was "pyawskit-0.1.77.tar", last modified: Thu Jul 13 05:31:07 2023, max compression
```

## Comparing `pyawskit-0.1.76.tar` & `pyawskit-0.1.77.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 04:39:11.481554 pyawskit-0.1.76/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-07-13 04:38:57.000000 pyawskit-0.1.76/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-13 04:39:11.481554 pyawskit-0.1.76/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-07-13 04:38:57.000000 pyawskit-0.1.76/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 04:39:11.481554 pyawskit-0.1.76/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.76/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.76/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.76/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.76/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3485 2023-07-13 04:38:19.000000 pyawskit-0.1.76/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.76/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.76/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14829 2023-04-27 08:16:18.000000 pyawskit-0.1.76/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.76/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      185 2023-07-13 04:38:57.000000 pyawskit-0.1.76/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.76/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 04:39:11.481554 pyawskit-0.1.76/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-07-13 04:39:11.000000 pyawskit-0.1.76/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-07-13 04:39:11.481554 pyawskit-0.1.76/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1761 2023-07-13 04:38:57.000000 pyawskit-0.1.76/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 05:31:07.720686 pyawskit-0.1.77/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-07-13 04:42:50.000000 pyawskit-0.1.77/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-13 05:31:07.720686 pyawskit-0.1.77/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-07-13 04:42:50.000000 pyawskit-0.1.77/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 05:31:07.720686 pyawskit-0.1.77/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.77/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.77/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.77/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.77/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3480 2023-07-13 05:30:12.000000 pyawskit-0.1.77/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.77/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.77/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14829 2023-04-27 08:16:18.000000 pyawskit-0.1.77/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.77/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      185 2023-07-13 04:42:50.000000 pyawskit-0.1.77/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.77/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-13 05:31:07.720686 pyawskit-0.1.77/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-07-13 05:31:07.000000 pyawskit-0.1.77/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-07-13 05:31:07.724686 pyawskit-0.1.77/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1761 2023-07-13 04:42:50.000000 pyawskit-0.1.77/setup.py
```

### Comparing `pyawskit-0.1.76/LICENSE` & `pyawskit-0.1.77/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/PKG-INFO` & `pyawskit-0.1.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.76
+Version: 0.1.77
 Summary: Pyawskit is your AWS Swiss Army Knife
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.76
+version: 0.1.77
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.76/pyawskit/aws.py` & `pyawskit-0.1.77/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.77/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.77/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/aws_ecr_login_code.py` & `pyawskit-0.1.77/pyawskit/aws_ecr_login_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import os.path
 import datetime
 import base64
 import subprocess
-from urllib.parse import urlparse, ParseResult
+from urllib.parse import urlparse
 import json
 
 # import requests.exceptions
 # import docker
 import boto3
 import pyapikey
 
@@ -34,29 +34,29 @@
             "login",
             "--username", user,
             "--password", password,
             proxyEndpoint,
         ])
 
 
-def strip_scheme(url):
+def strip_scheme(url: str) -> str:
     """ strip scheme from url
     References:
     - https://stackoverflow.com/questions/21687408/how-to-remove-scheme-from-url-in-python
     """
-    parsed_result = urlparse(url)
-    return ParseResult('', *parsed_result[1:]).geturl()
+    schemaless = urlparse(url)._replace(scheme='').geturl()
+    return schemaless[2:]
 
 
 def is_logged_in(proxyEndpoint: str) -> bool:
     """ return if you are currently logged in to a specific server
     References:
     - https://stackoverflow.com/questions/36022892/how-to-know-if-docker-is-already-logged-in-to-a-docker-registry-server
     """
-    config_file = os.path.expandvars("~/.docker/config.json")
+    config_file = os.path.expanduser("~/.docker/config.json")
     if os.path.isfile(config_file):
         with open(config_file, "r") as stream:
             data = json.load(stream)
             if "auths" not in data:
                 return False
             return strip_scheme(proxyEndpoint) in data["auths"]
     else:
```

### Comparing `pyawskit-0.1.76/pyawskit/common.py` & `pyawskit-0.1.77/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/configs.py` & `pyawskit-0.1.77/pyawskit/configs.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/main.py` & `pyawskit-0.1.77/pyawskit/main.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/os_utils.py` & `pyawskit-0.1.77/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit/utils.py` & `pyawskit-0.1.77/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.76/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.77/pyawskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.76
+Version: 0.1.77
 Summary: Pyawskit is your AWS Swiss Army Knife
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.76
+version: 0.1.77
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.76/setup.py` & `pyawskit-0.1.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.76",
+    version="0.1.77",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="Pyawskit is your AWS Swiss Army Knife",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

