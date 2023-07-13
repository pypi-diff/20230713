# Comparing `tmp/pyxecm-0.1.0.tar.gz` & `tmp/pyxecm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.1.0.tar", last modified: Wed Jul 12 13:06:50 2023, max compression
+gzip compressed data, was "pyxecm-0.1.1.tar", last modified: Thu Jul 13 17:23:38 2023, max compression
```

## Comparing `pyxecm-0.1.0.tar` & `pyxecm-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.292936 pyxecm-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-12 13:06:32.000000 pyxecm-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-12 13:06:50.292936 pyxecm-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-12 13:06:32.000000 pyxecm-0.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-12 13:06:40.000000 pyxecm-0.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.290936 pyxecm-0.1.0/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/assoc.py
--rw-rw-rw-   0 root         (0) root         (0)    33694 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     9554 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256462 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   129349 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10240 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/web.py
--rw-rw-rw-   0 root         (0) root         (0)    21848 2023-07-12 13:06:32.000000 pyxecm-0.1.0/pyxecm/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:06:50.291936 pyxecm-0.1.0/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 13:06:50.000000 pyxecm-0.1.0/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 13:06:50.292936 pyxecm-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-12 13:06:32.000000 pyxecm-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.685356 pyxecm-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-07-13 17:23:13.000000 pyxecm-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-13 17:23:38.685356 pyxecm-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-13 17:23:13.000000 pyxecm-0.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-13 17:23:28.000000 pyxecm-0.1.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.683356 pyxecm-0.1.1/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/assoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    33675 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)     9536 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256444 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   129331 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10222 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    21830 2023-07-13 17:23:13.000000 pyxecm-0.1.1/pyxecm/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:23:38.685356 pyxecm-0.1.1/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 17:23:38.000000 pyxecm-0.1.1/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:23:38.685356 pyxecm-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-13 17:23:13.000000 pyxecm-0.1.1/setup.py
```

### Comparing `pyxecm-0.1.0/LICENSE` & `pyxecm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.1.0/PKG-INFO` & `pyxecm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyxecm-0.1.0/README.md` & `pyxecm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.1.0/pyproject.toml` & `pyxecm-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "zipfile36", "suds"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
   keywords = ["opentext", "extendedecm", "contentserver", "otds", "appworks", "archivecenter"]
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.1.0"
+  version = "0.1.1"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.1.0/pyxecm/assoc.py` & `pyxecm-0.1.1/pyxecm/assoc.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.1.0/pyxecm/k8s.py` & `pyxecm-0.1.1/pyxecm/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,15 @@
 from kubernetes import client, config
 from kubernetes.stream import stream
 from kubernetes.client.exceptions import ApiException
 
 # Configure Kubernetes API authentication to use pod serviceAccount
 # config.load_incluster_config()
 
-logger = logging.getLogger(os.path.basename(__file__))
-
+logger = logging.getLogger("pyxecm")
 
 class K8s(object):
     """Used to automate stettings in Kubernetes."""
 
     _core_v1_api = None
     _apps_v1_api = None
     _networking_v1_api = None
```

### Comparing `pyxecm-0.1.0/pyxecm/otac.py` & `pyxecm-0.1.1/pyxecm/otac.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import requests
 import os
 import logging
 import base64
 
 from suds.client import Client
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 requestHeaders = {"Content-Type": "application/x-www-form-urlencoded"}
 
 
 class OTAC:
     """Used to automate stettings in OpenText Archive Center."""
```

### Comparing `pyxecm-0.1.0/pyxecm/otcs.py` & `pyxecm-0.1.1/pyxecm/otcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 import requests
 import json
 import urllib.parse
 from datetime import datetime
 import zipfile
 from .xml import XML
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
 requestFormHeaders = {
```

### Comparing `pyxecm-0.1.0/pyxecm/otds.py` & `pyxecm-0.1.1/pyxecm/otds.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 import os
 import logging
 import requests
 import json
 import base64
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 requestHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
 
 requestFormHeaders = {
```

### Comparing `pyxecm-0.1.0/pyxecm/otiv.py` & `pyxecm-0.1.1/pyxecm/otiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 __credits__ = ["Kai-Philip Gatzweiler"]
 __maintainer__ = "Dr. Marc Diefenbruch"
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 
 class OTIV(object):
     """Used to manage stettings for OpenText Intelligent Viewing."""
 
     _config = None
```

### Comparing `pyxecm-0.1.0/pyxecm/otpd.py` & `pyxecm-0.1.1/pyxecm/otpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import json
 import requests
 from requests.auth import HTTPBasicAuth
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 import os
 import logging
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 requestHeaders = {
     "accept": "application/json;charset=utf-8",
     "Connection": "keep-alive",
     "Content-Type": "application/json",
 }
```

### Comparing `pyxecm-0.1.0/pyxecm/web.py` & `pyxecm-0.1.1/pyxecm/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 __email__ = "mdiefenb@opentext.com"
 
 import requests
 import os
 import logging
 import socket
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 requestHeaders = {"Content-Type": "application/x-www-form-urlencoded"}
 
 
 class HTTP(object):
     """Used to automate stettings in OpenText Archive Center."""
```

### Comparing `pyxecm-0.1.0/pyxecm/xml.py` & `pyxecm-0.1.1/pyxecm/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # we need lxml instead of stadard xml.etree to have xpath capabilities!
 from lxml import etree
 
 # import xml.etree.ElementTree as etree
 from .assoc import Assoc
 
-logger = logging.getLogger(os.path.basename(__file__))
+logger = logging.getLogger("pyxecm")
 
 
 class XML:
     @classmethod
     def getXmlElement(cls, xml_content: str, xpath: str):
         # Parse XML content into an etree
         tree = etree.fromstring(xml_content)
```

### Comparing `pyxecm-0.1.0/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.1.1/pyxecm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://ecm.glpages.otxlab.net/pyxecm/
 Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

