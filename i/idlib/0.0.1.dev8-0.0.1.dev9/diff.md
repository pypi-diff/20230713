# Comparing `tmp/idlib-0.0.1.dev8.tar.gz` & `tmp/idlib-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/idlib-0.0.1.dev8.tar", last modified: Tue Oct 20 21:30:52 2020, max compression
+gzip compressed data, was "idlib-0.0.1.dev9.tar", last modified: Sat May  1 04:52:38 2021, max compression
```

## Comparing `idlib-0.0.1.dev8.tar` & `idlib-0.0.1.dev9.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.980039 idlib-0.0.1.dev8/
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1121 2020-10-20 21:30:52.980039 idlib-0.0.1.dev8/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      148 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/Pipfile
--rw-r--r--   0 tom       (1000) tom       (1000)      406 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.976039 idlib-0.0.1.dev8/docs/
--rw-r--r--   0 tom       (1000) tom       (1000)     4835 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/docs/identifiers.org
--rw-r--r--   0 tom       (1000) tom       (1000)     1441 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/docs/stream-grammer.org
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.977039 idlib-0.0.1.dev8/idlib/
--rw-r--r--   0 tom       (1000) tom       (1000)     1662 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.978039 idlib-0.0.1.dev8/idlib/apis/
--rw-r--r--   0 tom       (1000) tom       (1000)       88 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/apis/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3388 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/apis/protocols_io.py
--rw-r--r--   0 tom       (1000) tom       (1000)      419 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/auth-config.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3446 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/cache.py
--rw-r--r--   0 tom       (1000) tom       (1000)       76 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/config.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.978039 idlib-0.0.1.dev8/idlib/conventions/
--rw-r--r--   0 tom       (1000) tom       (1000)      204 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/conventions/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      940 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/conventions/core.py
--rw-r--r--   0 tom       (1000) tom       (1000)      129 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/conventions/local.py
--rw-r--r--   0 tom       (1000) tom       (1000)      814 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/conventions/type.py
--rw-r--r--   0 tom       (1000) tom       (1000)      864 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/core.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1719 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/exceptions.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.979039 idlib-0.0.1.dev8/idlib/formats/
--rw-r--r--   0 tom       (1000) tom       (1000)      528 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/formats/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      466 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/formats/rdf.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25960 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/from_oq.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3763 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/identifiers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    20881 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/streams.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.980039 idlib-0.0.1.dev8/idlib/systems/
--rw-r--r--   0 tom       (1000) tom       (1000)      180 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      111 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/ark.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10503 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/doi.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/handle.py
--rw-r--r--   0 tom       (1000) tom       (1000)       89 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/isni.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6584 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/orcid.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7082 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/ror.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5679 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/rrid.py
--rw-r--r--   0 tom       (1000) tom       (1000)      113 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/urn.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1291 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/systems/web.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3327 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/idlib/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.978039 idlib-0.0.1.dev8/idlib.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1121 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      948 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       20 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      192 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        6 2020-10-20 21:30:52.000000 idlib-0.0.1.dev8/idlib.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2020-10-20 21:30:52.981039 idlib-0.0.1.dev8/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1788 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-10-20 21:30:52.980039 idlib-0.0.1.dev8/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1172 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/test/test_cache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8922 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/test/test_identifiers.py
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2020-09-30 21:48:05.000000 idlib-0.0.1.dev8/test/test_simple.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.424263 idlib-0.0.1.dev9/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1121 2021-05-01 04:52:38.424263 idlib-0.0.1.dev9/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      148 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/Pipfile
+-rw-r--r--   0 tom       (1000) tom       (1000)      406 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.421263 idlib-0.0.1.dev9/docs/
+-rw-r--r--   0 tom       (1000) tom       (1000)    17645 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/docs/identifiers.org
+-rw-r--r--   0 tom       (1000) tom       (1000)     1441 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/docs/stream-grammer.org
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.422263 idlib-0.0.1.dev9/idlib/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1695 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.422263 idlib-0.0.1.dev9/idlib/apis/
+-rw-r--r--   0 tom       (1000) tom       (1000)       88 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/apis/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3558 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/apis/protocols_io.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      419 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/auth-config.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3446 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/cache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       76 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/config.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.423263 idlib-0.0.1.dev9/idlib/conventions/
+-rw-r--r--   0 tom       (1000) tom       (1000)      204 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/conventions/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      940 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/conventions/core.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      129 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/conventions/local.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      814 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/conventions/type.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1055 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/core.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3635 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/edit.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3816 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/exceptions.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.423263 idlib-0.0.1.dev9/idlib/formats/
+-rw-r--r--   0 tom       (1000) tom       (1000)      528 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/formats/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      466 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/formats/rdf.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    28993 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/from_oq.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3763 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/identifiers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    21552 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/streams.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.424263 idlib-0.0.1.dev9/idlib/systems/
+-rw-r--r--   0 tom       (1000) tom       (1000)      203 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      111 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/ark.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10533 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/doi.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/handle.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       89 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/isni.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6584 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/orcid.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      181 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/pmid.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7816 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/ror.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5679 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/rrid.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      113 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/urn.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1291 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/systems/web.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3327 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/idlib/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.422263 idlib-0.0.1.dev9/idlib.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1121 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      984 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       20 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      192 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        6 2021-05-01 04:52:38.000000 idlib-0.0.1.dev9/idlib.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2021-05-01 04:52:38.424263 idlib-0.0.1.dev9/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1788 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2021-05-01 04:52:38.424263 idlib-0.0.1.dev9/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1172 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/test/test_cache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9009 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/test/test_identifiers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2021-05-01 04:50:15.000000 idlib-0.0.1.dev9/test/test_simple.py
```

### Comparing `idlib-0.0.1.dev8/LICENSE` & `idlib-0.0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/PKG-INFO` & `idlib-0.0.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlib
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: A library for working with identifiers of all kinds.
 Home-page: https://github.com/tgbugs/idlib
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # idlib
         [![PyPI version](https://badge.fury.io/py/idlib.svg)](https://pypi.org/project/idlib/)
```

### Comparing `idlib-0.0.1.dev8/docs/stream-grammer.org` & `idlib-0.0.1.dev9/docs/stream-grammer.org`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/__init__.py` & `idlib-0.0.1.dev9/idlib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from idlib.from_oq import (Auto,
                            Pio,
                            PioUser,)
 from idlib.systems import (Ark,
                            Doi,
                            Handle,
                            Orcid,
+                           Pmid,
                            Ror,
                            Rrid,
                            Uri,
                            Urn,)
 
 # assign default identifier classes to streams
 StreamUri._id_class = Uri
@@ -50,8 +51,8 @@
                 pi = StreamUriTemp(uri)
         else:
             pi = uri
 
     return pi
 
 
-__version__ = '0.0.1.dev8'
+__version__ = '0.0.1.dev9'
```

### Comparing `idlib-0.0.1.dev8/idlib/apis/protocols_io.py` & `idlib-0.0.1.dev9/idlib/apis/protocols_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,17 @@
     code = params['code']
     return code
 
 
 def get_protocols_io_auth(creds_file,
                           store_file=auth.get_path('protocols-io-api-store-file'),
                           SCOPES='readwrite'):
-
     from google_auth_oauthlib.flow import InstalledAppFlow
     from google.auth.transport.requests import Request
+    from idlib import exceptions as exc
 
     InstalledAppFlowConsole = type('InstalledAppFlowConsole',
                                    (ConsoleHelper, InstalledAppFlow),
                                    {})
     if store_file.exists():
         with open(store_file, 'rb') as f:
             try:
@@ -87,15 +87,18 @@
                 log.error(f'problem in file at path for "protocols-io-api-store-file"')
                 raise e
     else:
         creds = None
 
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
-            creds.refresh(Request())
+            try:
+                creds.refresh(Request())
+            except Exception as e:
+                raise exc.RemoteError('protocols.io refresh error') from e
         else:
             flow = InstalledAppFlowConsole.from_client_secrets_file(creds_file.as_posix(), SCOPES)
             creds = flow.run_console_only()
 
         with open(store_file, 'wb') as f:
             pickle.dump(creds, f)
```

### Comparing `idlib-0.0.1.dev8/idlib/cache.py` & `idlib-0.0.1.dev9/idlib/cache.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/conventions/core.py` & `idlib-0.0.1.dev9/idlib/conventions/core.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/conventions/type.py` & `idlib-0.0.1.dev9/idlib/conventions/type.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/core.py` & `idlib-0.0.1.dev9/idlib/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 def resolution_chain_responses(iri, raise_on_final=True):
     #doi = doi  # TODO
     s = requests.Session()
     head = requests.head(iri)
     yield head
     while head.is_redirect and head.status_code < 400:  # FIXME redirect loop issue
         yield head.next
-        head = s.send(head.next)
+        try:
+            head = s.send(head.next)
+        except requests.exceptions.SSLError as e:
+            raise exc.InbetweenError(msg) from e
+
         yield head
         if not head.is_redirect:
             break
 
     if raise_on_final:  # we still want the chain ... null pointer error comes later?
         if head.status_code == 404:
             head.raise_for_status()  # probably a permissions issue
+        elif head.status_code >= 500:
+            raise exc.RemoteError()
         elif head.status_code >= 400:
             msg = f'Nothing found due to {head.status_code} at {head.url}\n'
             raise exc.ResolutionError(msg)
```

### Comparing `idlib-0.0.1.dev8/idlib/formats/__init__.py` & `idlib-0.0.1.dev9/idlib/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/from_oq.py` & `idlib-0.0.1.dev9/idlib/from_oq.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from datetime import datetime
 #import requests
 import orthauth as oa
 import ontquery as oq  # temporary implementation detail
 import idlib
 from idlib import apis
+from idlib import formats
 from idlib import streams
 from idlib import exceptions as exc
 from idlib import conventions as conv
 from idlib.cache import cache, COOLDOWN
 from idlib.utils import (log,
                          TZLOCAL,
                          cache_result,
@@ -273,15 +274,15 @@
                             ' unless you have it in secrets') from e
 
     _pio_creds = apis.protocols_io.get_protocols_io_auth(creds_file)
     cls._pio_header = oa.utils.QuietDict(
         {'Authorization': 'Bearer ' + _pio_creds.token})
 
 
-class Pio(idlib.Stream):
+class Pio(formats.Rdf, idlib.Stream):
     """ instrumented protocols """
 
     _id_class = PioId
     # FIXME defining this here breaks the import chain
     # since protocols.py imports from core.py (sigh)
     _wants_instance = '.protocols.ProtocolData'  # this is an awful pattern
     # but what do you want :/
@@ -290,14 +291,22 @@
     dereference_chain = streams.StreamUri.dereference_chain
     dereference = streams.StreamUri.dereference
     progenitor = streams.StreamUri.progenitor
     headers = streams.StreamUri.headers
 
     _setup = classmethod(setup)
 
+    #_checked_whether_data_is_not_in_error = False
+    #_data_is_in_error = True
+    # we MUST assume that data is in error for all instances by
+    # default until they prove otherwise HOWEVER the problem is that
+    # you now also need another parameter which is whether you have
+    # checked to see if it is NOT in error, sigh maybe in error? sigh
+    # this becomes hasattr(self, '_data_in_error) and self._data_in_error
+
     def __new__(cls, *args, **kwargs):
         # sadly it seems that this has to be defined explicitly
         return super().__new__(cls)
 
     __new__rest = __new__
 
     def __new__(cls, *args, **kwargs):
@@ -335,15 +344,30 @@
             if doi:
                 return idlib.Doi(doi)
 
     @property
     @cache_result  # caching this cuts time in half for 2 calls etc. 5s / 10s over 25k calls
     def uri_human(self):  # FIXME HRM ... confusion with pio.private iris
         """ the not-private uri """
-        data = self.data()
+        try:
+            data = self.data()
+        except exc.RemoteError as e:
+            data = None
+            try:
+                proj = self.progenitor(type='id-converted-from')
+                # it should not be the case that we somehow find a
+                # private id here because data would have traversed
+                # and found it already and gotten the metadata
+                # FIXME doi, other int, private should all not be here
+                if not proj.identifier.is_int():
+                    return proj
+                else:
+                    raise e
+            except KeyError as e2:
+                raise e
         if data:
             uri = data['uri']
             if uri:
                 return self.fromIdInit(prefix='pio.view', suffix=uri)
 
     id_bound_metadata = uri_human  # FIXME vs uri field
     identifier_bound_metadata = id_bound_metadata
@@ -387,14 +411,15 @@
             pid._progenitors = {}
 
         pid._progenitors['id-converted-from'] = self
         return pid
 
     def data(self, fail_ok=False):
         if not hasattr(self, '_data'):
+            self._data_in_error = True
             if not isinstance(self._progenitors, dict):
                 # XXX careful about the contents going stale
                 self._progenitors = {}
 
             apiuri = self.identifier.uri_api
             blob, path = self._get_data(apiuri)
             if 'stream-http' not in self._progenitors:
@@ -411,23 +436,35 @@
                     raise NotImplementedError('asdf')
 
                 sc = blob['pio_status_code']
                 if sc == 212:  # Protocol does not exist
                     if fail_ok: return
                     raise exc.IdDoesNotExistError(message)
                 elif sc in (250, 205):  # access requested, not authorized
+                    try:
+                        # there might be a private id in the progenitor chain
+                        nself = self.progenitor(type='id-converted-from')
+                        # FIXME TODO this works, but it would be nice if we
+                        # could use this to populate the cache for the public
+                        # api identifier as well
+                        return nself.data(fail_ok=fail_ok)
+                    except KeyError as e:
+                        pass
+
                     if fail_ok: return
                     raise exc.NotAuthorizedError(message)
                 else:
                     msg = f'unhandled pio status code {sc}\n' + message
                     raise NotImplementedError(msg)
             else:
                 self._status_code = blob['status_code']
                 self._data = blob['protocol']
 
+            self._data_in_error = False
+
         return self._data
 
     @cache(auth.get_path('cache-path') / 'protocol_json', create=True, return_path=True)
     def _get_data(self, apiuri):
         """ use apiuri as the identifier since it is distinct
             from other views of the protocol e.g. uri_human etc. """
 
@@ -542,17 +579,31 @@
 
     def asUri(self, asType=None):
         return (self.identifier.iri
                 if asType is None else
                 asType(self.identifier.iri))
 
     def asDict(self, include_description=False, include_private=True):
+        """ XXX this should NEVER allow an error to escape.
+            Only return less information. """
         if self.identifier.is_int():
             out = super().asDict(include_description)
-            out['uri_human'] = self.uri_human.identifier  # prevent double embedding
+
+            try:
+                out['uri_human'] = self.uri_human.identifier  # prevent double embedding
+            except exc.RemoteError as e:
+                pass
+
+            if hasattr(self, '_data_in_error') and self._data_in_error:
+                return out
+
+            # NOTE if you started from a doi then it seems extremely unlikely
+            # that you would be in a sitution where data retrieval could fail
+            # which means that really only the uri_human case can fail and
+            # there still be a chance that there is a uri_human we can use
             doi = self.doi
             if doi is not None:
                 out['doi'] = doi
             return out
         else:
             try:
                 uri_api_int = self.uri_api_int
@@ -565,14 +616,39 @@
                 if include_private and self.identifier.is_private():
                     out['uri_private'] = self.identifier  # FIXME some way to avoid leaking these if needed?
                 return out
             except exc.RemoteError as e:
                 # we don't have any metadata but we will return what little info we have
                 return super().asDict(include_description)
 
+    def _triples_gen(self,
+                     rdflib=None,
+                     rdf=None,
+                     rdfs=None,
+                     owl=None,
+                     NIFRID=None,
+                     TEMP=None,
+                     **kwargs):
+
+        s = self.asType(rdflib.URIRef)
+
+        yield s, rdf.type, owl.NamedIndividual
+
+        if self.uri_human:
+            # XXX dereference checks should not be run here, they
+            # should be conduceded centrally during
+            yield s, TEMP.hasUriHuman, self.uri_human.asType(rdflib.URIRef)
+
+        if self.label:
+            yield s, rdfs.label, rdflib.Literal(self.label)
+
+        doi = self.doi
+        if doi is not None:
+            yield s, TEMP.hasDoi, doi.asType(rdflib.URIRef)
+
 
 class _PioUserPrefixes(conv.QnameAsLocalHelper, oq.OntCuries):
     # set these manually since, sigh, factory patterns
     _dict = {}
     _n_to_p = {}
     _strie = {}
     _trie = {}
```

### Comparing `idlib-0.0.1.dev8/idlib/identifiers.py` & `idlib-0.0.1.dev9/idlib/identifiers.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/streams.py` & `idlib-0.0.1.dev9/idlib/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,16 @@
             return self.label + sep + local
 
         else:
             # FIXME this needs some extension mechanism ...
             raise NotImplementedError('TODO as needed')
 
     def asDict(self, include_description=False):
+        """ XXX this should NEVER allow an error to escape.
+            Only return less information. """
         if hasattr(self, '_id_class') and self._id_class:
             out = {
                 'type': 'identifier',
                 'system': self.__class__.__name__,
                 #'id': self.identifier,
                 'id': self,  # XXX NOTE THE TRADEOFF HERE, this preserves stream access
                 # 'alternate_identifiers': [],  # TODO
@@ -251,15 +253,15 @@
             note that sometimes this may include a tuple if the information
             needed has more than one part, no conventions for this have
             been decided yet
 
             level == 0 -> returns self to break"""
 
         if args:
-            raise TypeError('progenitor acceps keywords arguments only!')
+            raise TypeError('progenitor accepts keywords arguments only!')
 
         # FIXME probably makes more sense to store progenitors in a dict
         # with a controlled set of types than just by accident of ordering
         # this would allow us to keep everything along the way
         # of course watch out for garbage collection issues ala lxml etree
 
         # XXX NOTE: self._progenitors = [] should be set EVERY time data is retrieved
@@ -475,15 +477,27 @@
         return dc[self.identifier_actionable]
 
     @cache_result
     def dereference(self, asType=None):
         drc = self.dereference_chain()
         uri = drc[-1]
         if asType:
-            return asType(uri)
+            nid = asType(uri)
+            if isinstance(nid, idlib.Stream):
+                if not isinstance(nid._progenitors, dict):
+                    # FIXME is are these really progenitors in the way we usually
+                    # think of them? ... maybe not?
+                    nid._progenitors = {}
+
+                # FIXME TODO do we want/need the full chain here?
+                nid._progenitors['id-dereferenced-from'] = self
+                # FIXME temporary bridge from StringProgenitor
+                nid._progenitors['stream-http'] = uri._progenitor
+
+            return nid
         else:
             # just return the strprg if no type is set
             # don't assume dereferencing is type preserving
             # if we wanted to be really strict about types then we would force
             # explicit conversion to a actionable form and then dereference
             # i.e. ident.actionable().dereference() but that is a pain since
             # the original stream object looses its connection, and the identifier
```

### Comparing `idlib-0.0.1.dev8/idlib/systems/doi.py` & `idlib-0.0.1.dev9/idlib/systems/doi.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     # additional streams ...
 
     def ttl(self):  # this is another potential way to deal with mimetypes
         # both datacite and crossref produce in turtle
         resp = self._requests.get(self.identifier, headers={'Accept': 'text/turtle'})
         self._ttl_resp = resp
-        ct = resp.headers['Content-Type']
+        ct = resp.headers['Content-Type']  # FIXME this can KeyError !?
         if 'text/html' in ct:
             # sigh blackfynn
             log.warning(f'{resp.url} is not turtle it is {ct}')  # FIXME duplicate log messages happen here
             return
         else:
             return resp.text
```

### Comparing `idlib-0.0.1.dev8/idlib/systems/orcid.py` & `idlib-0.0.1.dev9/idlib/systems/orcid.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/systems/ror.py` & `idlib-0.0.1.dev9/idlib/systems/ror.py`

 * *Files 11% similar despite different names*

```diff
@@ -112,19 +112,34 @@
     def _metadata(self, suffix):
         # TODO data endpoint prefix ??
         # vs data endpoint pattern ...
         prefix = 'ror.api'  # NOTE THE CHANGE IN PREFIX
         idq = self._id_class(prefix=prefix, suffix=suffix)
         self._resp_metadata = self._requests.get(idq)
         if self._resp_metadata.ok:
-            return self._resp_metadata.json()
+            blob = self._resp_metadata.json()
+            if len(blob) == 1 and 'errors' in blob:
+                errors = blob['errors']
+                if len(errors) == 1:
+                    error = errors[0]
+                    if 'does not exist' in error:
+                        # FIXME pretty sure this should be a used to
+                        # exist error in the example that causes this
+                        raise exc.IdDoesNotExistError(self.identifier)
+                    else:
+                        raise exc.RemoteError(error)
+                else:
+                    raise exc.RemoteError(' '.join(errors))
+            else:
+                return blob
         else:
             try:
                 self._resp_metadata.raise_for_status()
             except BaseException as e:
+                # FIXME may not be a resolution error
                 raise exc.ResolutionError(identifier) from e
 
     @property
     def name(self):
         return self.metadata()['name']
 
     def asExternalId(self, id_class):
@@ -171,15 +186,15 @@
                      NIFRID=None,
                      TEMP=None,
                      **kwargs):
         """ implementation of method to produce a
             triplified version of the record """
         s = self.asType(rdflib.URIRef)
         a = rdf.type
-        yield s, a, owl.NamedIndividual
+        yield s, a, owl.NamedIndividual  # this goes first in the event the rest fail
         for osuffix in self.institutionTypes:
             o = TEMP[osuffix]
             yield s, a, o
 
         yield s, rdfs.label, rdflib.Literal(self.label)
         for o in self.synonyms_rdf(rdflib):
             yield s, NIFRID.synonym, o  # FIXME this looses information about synonym type
```

### Comparing `idlib-0.0.1.dev8/idlib/systems/rrid.py` & `idlib-0.0.1.dev9/idlib/systems/rrid.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/systems/web.py` & `idlib-0.0.1.dev9/idlib/systems/web.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib/utils.py` & `idlib-0.0.1.dev9/idlib/utils.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/idlib.egg-info/PKG-INFO` & `idlib-0.0.1.dev9/idlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlib
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: A library for working with identifiers of all kinds.
 Home-page: https://github.com/tgbugs/idlib
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # idlib
         [![PyPI version](https://badge.fury.io/py/idlib.svg)](https://pypi.org/project/idlib/)
```

### Comparing `idlib-0.0.1.dev8/idlib.egg-info/SOURCES.txt` & `idlib-0.0.1.dev9/idlib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 docs/identifiers.org
 docs/stream-grammer.org
 idlib/__init__.py
 idlib/auth-config.py
 idlib/cache.py
 idlib/config.py
 idlib/core.py
+idlib/edit.py
 idlib/exceptions.py
 idlib/from_oq.py
 idlib/identifiers.py
 idlib/streams.py
 idlib/utils.py
 idlib.egg-info/PKG-INFO
 idlib.egg-info/SOURCES.txt
@@ -31,14 +32,15 @@
 idlib/formats/rdf.py
 idlib/systems/__init__.py
 idlib/systems/ark.py
 idlib/systems/doi.py
 idlib/systems/handle.py
 idlib/systems/isni.py
 idlib/systems/orcid.py
+idlib/systems/pmid.py
 idlib/systems/ror.py
 idlib/systems/rrid.py
 idlib/systems/urn.py
 idlib/systems/web.py
 test/__init__.py
 test/test_cache.py
 test/test_identifiers.py
```

### Comparing `idlib-0.0.1.dev8/setup.py` & `idlib-0.0.1.dev9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
           'idlib.apis',
           'idlib.conventions',
           'idlib.formats',
           'idlib.systems',
       ],
       python_requires='>=3.6',
       tests_require=tests_require,
-      install_requires=['orthauth>=0.0.13[yaml]', 'requests'],
+      install_requires=['orthauth[yaml]>=0.0.13', 'requests'],
       extras_require={'test': tests_require,
                       'rdf': rdf_require,
                       'oauth': oauth_require,
                      },
       scripts=[],
       entry_points={'console_scripts': [ ],},
      )
```

### Comparing `idlib-0.0.1.dev8/test/test_cache.py` & `idlib-0.0.1.dev9/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `idlib-0.0.1.dev8/test/test_identifiers.py` & `idlib-0.0.1.dev9/test/test_identifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,17 @@
 class TestRor(HelperStream, unittest.TestCase):
     stream = idlib.Ror
     ids = [
         'https://ror.org/0168r3w48',
         'https://ror.org/02dqehb95',
         'https://ror.org/051fd9666',
     ]
-    ids_bad = []
+    ids_bad = [
+        'https://ror.org/05ht4p406',  # used to exist but api won't tell you that
+    ]
     for __i in ids:  # LOL PYTHON class scope list comprehensions
         ids_bad.append(__i.replace('https', 'http'))
     del __i
 
     def test_init(self):
         ic = idlib.Ror._id_class
         r = idlib.Ror._id_class(prefix='ror.api', suffix='0168r3w48')
```

