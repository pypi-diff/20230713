# Comparing `tmp/pymantic-0.3.0.tar.gz` & `tmp/pymantic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymantic-0.3.0.tar", last modified: Mon Jan  4 22:00:35 2021, max compression
+gzip compressed data, was "pymantic-1.0.0.tar", last modified: Thu Jul 13 16:29:00 2023, max compression
```

## Comparing `pymantic-0.3.0.tar` & `pymantic-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,46 @@
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/
--rw-r--r--   0 npilon    (1000) npilon    (1000)     2496 2021-01-04 22:00:35.507614 pymantic-0.3.0/PKG-INFO
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1226 2021-01-04 21:58:56.000000 pymantic-0.3.0/README.rst
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/
--rw-r--r--   0 npilon    (1000) npilon    (1000)       38 2021-01-04 21:58:56.000000 pymantic-0.3.0/pymantic/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1983 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/change_tracking.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    32396 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/compat.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/parsers/
--rw-r--r--   0 npilon    (1000) npilon    (1000)      206 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/parsers/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1656 2021-01-04 21:58:56.000000 pymantic-0.3.0/pymantic/parsers/base.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     2625 2020-03-27 16:07:19.000000 pymantic-0.3.0/pymantic/parsers/jsonld.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/parsers/lark/
--rw-r--r--   0 npilon    (1000) npilon    (1000)      190 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/parsers/lark/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1455 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/parsers/lark/base.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1198 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/parsers/lark/nquads.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     3188 2021-01-04 21:58:56.000000 pymantic-0.3.0/pymantic/parsers/lark/ntriples.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    11044 2021-01-04 21:58:56.000000 pymantic-0.3.0/pymantic/parsers/lark/turtle.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     3254 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/parsers/rdfxml.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    27687 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/primitives.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    24329 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/rdf.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/scripts/
--rw-r--r--   0 npilon    (1000) npilon    (1000)        0 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/scripts/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     9450 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/scripts/bnf2html
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1287 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/scripts/named_graph_to_nquads
--rw-r--r--   0 npilon    (1000) npilon    (1000)     6050 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/serializers.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    12306 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/sparql.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/tests/
--rw-r--r--   0 npilon    (1000) npilon    (1000)        0 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    35270 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_RDF.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1537 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_SPARQL.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     6428 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_parsers.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     6016 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_primitives.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)    10914 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_serializers.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     4504 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_turtle.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1340 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/tests/test_util.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)      822 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/uri_schemes.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)     3359 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/util.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic/vocab/
--rw-r--r--   0 npilon    (1000) npilon    (1000)        0 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/vocab/__init__.py
--rw-r--r--   0 npilon    (1000) npilon    (1000)      378 2019-07-10 16:42:04.000000 pymantic-0.3.0/pymantic/vocab/skos.py
-drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2021-01-04 22:00:35.503614 pymantic-0.3.0/pymantic.egg-info/
--rw-r--r--   0 npilon    (1000) npilon    (1000)     2496 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/PKG-INFO
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1101 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/SOURCES.txt
--rw-r--r--   0 npilon    (1000) npilon    (1000)        1 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/dependency_links.txt
--rw-r--r--   0 npilon    (1000) npilon    (1000)       37 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/entry_points.txt
--rw-r--r--   0 npilon    (1000) npilon    (1000)        1 2019-07-10 16:42:36.000000 pymantic-0.3.0/pymantic.egg-info/not-zip-safe
--rw-r--r--   0 npilon    (1000) npilon    (1000)       92 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/requires.txt
--rw-r--r--   0 npilon    (1000) npilon    (1000)        9 2021-01-04 22:00:35.000000 pymantic-0.3.0/pymantic.egg-info/top_level.txt
--rw-r--r--   0 npilon    (1000) npilon    (1000)       62 2021-01-04 22:00:35.507614 pymantic-0.3.0/setup.cfg
--rw-r--r--   0 npilon    (1000) npilon    (1000)     1784 2021-01-04 21:58:56.000000 pymantic-0.3.0/setup.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.417355 pymantic-1.0.0/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1608 2023-07-13 16:28:28.000000 pymantic-1.0.0/LICENSE
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     2057 2023-07-13 16:29:00.417355 pymantic-1.0.0/PKG-INFO
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1226 2023-07-13 16:28:28.000000 pymantic-1.0.0/README.rst
+-rw-r--r--   0 npilon    (1000) npilon    (1000)      561 2023-07-13 16:28:28.000000 pymantic-1.0.0/pyproject.toml
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1102 2023-07-13 16:29:00.417355 pymantic-1.0.0/setup.cfg
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.409355 pymantic-1.0.0/src/
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)       38 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/__init__.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic/parsers/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)      180 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/__init__.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1648 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/base.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     2652 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/jsonld.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic/parsers/lark/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)      190 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/lark/__init__.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1382 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/lark/base.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1170 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/lark/nquads.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     3139 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/lark/ntriples.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    10874 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/lark/turtle.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     3253 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/parsers/rdfxml.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    27360 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/primitives.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    24563 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/rdf.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic/scripts/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/scripts/__init__.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     5947 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/serializers.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    12387 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/sparql.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1120 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/uri_schemes.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     3281 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/util.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic/vocab/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/vocab/__init__.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)      375 2023-07-13 16:28:28.000000 pymantic-1.0.0/src/pymantic/vocab/skos.py
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.413355 pymantic-1.0.0/src/pymantic.egg-info/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     2057 2023-07-13 16:29:00.000000 pymantic-1.0.0/src/pymantic.egg-info/PKG-INFO
+-rw-r--r--   0 npilon    (1000) npilon    (1000)      974 2023-07-13 16:29:00.000000 pymantic-1.0.0/src/pymantic.egg-info/SOURCES.txt
+-rw-r--r--   0 npilon    (1000) npilon    (1000)        1 2023-07-13 16:29:00.000000 pymantic-1.0.0/src/pymantic.egg-info/dependency_links.txt
+-rw-r--r--   0 npilon    (1000) npilon    (1000)       85 2023-07-13 16:29:00.000000 pymantic-1.0.0/src/pymantic.egg-info/requires.txt
+-rw-r--r--   0 npilon    (1000) npilon    (1000)        9 2023-07-13 16:29:00.000000 pymantic-1.0.0/src/pymantic.egg-info/top_level.txt
+-rw-r--r--   0 npilon    (1000) npilon    (1000)        1 2023-07-06 13:24:57.000000 pymantic-1.0.0/src/pymantic.egg-info/zip-safe
+drwxr-xr-x   0 npilon    (1000) npilon    (1000)        0 2023-07-13 16:29:00.417355 pymantic-1.0.0/tests/
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    32209 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_RDF.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1361 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_SPARQL.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     6914 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_parsers.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     6569 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_primitives.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)    10342 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_serializers.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     3885 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_turtle.py
+-rw-r--r--   0 npilon    (1000) npilon    (1000)     1349 2023-07-13 16:28:28.000000 pymantic-1.0.0/tests/test_util.py
```

### Comparing `pymantic-0.3.0/PKG-INFO` & `pymantic-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: pymantic
-Version: 0.3.0
+Version: 1.0.0
 Summary: Semantic Web and RDF library for Python
 Home-page: https://github.com/norcalrdf/pymantic/
 Author: Gavin Carothers, Nick Pilon
 Author-email: gavin@carothers.name, npilon@gmail.com
 License: BSD
-Description: ========
-        Pymantic
-        ========
-        ---------------------------------------
-        Semantic Web and RDF library for Python
-        ---------------------------------------
-        
-        
-        Quick Start
-        ===========
-        ::
-        
-            >>> from pymantic.rdf import *
-            >>> from pymantic.parsers import turtle_parser
-            >>> import requests
-            >>> Resource.prefixes['foaf'] = Prefix('http://xmlns.com/foaf/0.1/')
-            >>> graph = turtle_parser.parse(requests.get('https://raw.github.com/norcalrdf/pymantic/master/examples/foaf-bond.ttl').text)
-            >>> bond_james = Resource(graph, 'http://example.org/stuff/Bond')
-            >>> print("%s knows:" % (bond_james.get_scalar('foaf:name'),))
-            >>> for person in bond_james['foaf:knows']:
-                    print(person.get_scalar('foaf:name'))
-        
-        
-        
-        Requirements
-        ============
-        
-        ``pymantic`` requires Python 3.6 or higher.
-        ``lark`` is used for the Turtle and NTriples parser.
-        The ``requests`` library is used for HTTP requests and the SPARQL client.
-        ``lxml`` and ``rdflib`` are required by the SPARQL client as well.
-        
-        
-        Install
-        =======
-        
-        ::
-        
-            $ pip install pymantic
-        
-        This will install ``pymantic`` and all its dependencies.
-        
-        
-        Documentation
-        =============
-        
-        Generating a local copy of the documentation requires Sphinx:
-        
-        ::
-        
-            $ pip install Sphinx
-        
-        
-        
-Keywords: RDF N3 Turtle Semantics Web3.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Keywords: RDF N3 Turtle Semantics
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Markup
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
+License-File: LICENSE
+
+========
+Pymantic
+========
+---------------------------------------
+Semantic Web and RDF library for Python
+---------------------------------------
+
+
+Quick Start
+===========
+::
+
+    >>> from pymantic.rdf import *
+    >>> from pymantic.parsers import turtle_parser
+    >>> import requests
+    >>> Resource.prefixes['foaf'] = Prefix('http://xmlns.com/foaf/0.1/')
+    >>> graph = turtle_parser.parse(requests.get('https://raw.github.com/norcalrdf/pymantic/master/examples/foaf-bond.ttl').text)
+    >>> bond_james = Resource(graph, 'http://example.org/stuff/Bond')
+    >>> print("%s knows:" % (bond_james.get_scalar('foaf:name'),))
+    >>> for person in bond_james['foaf:knows']:
+            print(person.get_scalar('foaf:name'))
+
+
+
+Requirements
+============
+
+``pymantic`` requires Python 3.9 or higher.
+``lark`` is used for the Turtle and NTriples parser.
+The ``requests`` library is used for HTTP requests and the SPARQL client.
+``lxml`` and ``rdflib`` are required by the SPARQL client as well.
+
+
+Install
+=======
+
+::
+
+    $ pip install pymantic
+
+This will install ``pymantic`` and all its dependencies.
+
+
+Documentation
+=============
+
+Generating a local copy of the documentation requires Sphinx:
+
+::
+
+    $ pip install Sphinx
+
+
```

### Comparing `pymantic-0.3.0/README.rst` & `pymantic-1.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             print(person.get_scalar('foaf:name'))
 
 
 
 Requirements
 ============
 
-``pymantic`` requires Python 3.6 or higher.
+``pymantic`` requires Python 3.9 or higher.
 ``lark`` is used for the Turtle and NTriples parser.
 The ``requests`` library is used for HTTP requests and the SPARQL client.
 ``lxml`` and ``rdflib`` are required by the SPARQL client as well.
 
 
 Install
 =======
```

### Comparing `pymantic-0.3.0/pymantic/parsers/base.py` & `pymantic-1.0.0/src/pymantic/parsers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from threading import local
 
 import pymantic.primitives
 
 
-class BaseParser(object):
+class BaseParser:
     """Common base class for all parsers
 
     Provides shared utilities for creating RDF objects, handling IRIs, and
     tracking parser state.
     """
 
     def __init__(self, environment=None):
```

### Comparing `pymantic-0.3.0/pymantic/parsers/jsonld.py` & `pymantic-1.0.0/src/pymantic/parsers/jsonld.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import json
 
 from .base import BaseParser
 
 
 class PyLDLoader(BaseParser):
-    class _Loader(object):
+    class _Loader:
         def __init__(self, pyld_loader):
             self.pyld_loader = pyld_loader
 
         def parse_file(self, f):
             jobj = json.load(f)
             self.pyld_loader.process_jobj(jobj)
 
@@ -42,41 +42,43 @@
         return self.env.createDataset()
 
     def __init__(self, *args, **kwargs):
         self.document = self._Loader(self)
         super(PyLDLoader, self).__init__(*args, **kwargs)
 
     def process_triple_fragment(self, triple_fragment):
-        if triple_fragment['type'] == 'IRI':
-            return self.env.createNamedNode(triple_fragment['value'])
-        elif triple_fragment['type'] == 'blank node':
-            return self._call_state.bnodes[triple_fragment['value']]
-        elif triple_fragment['type'] == 'literal':
+        if triple_fragment["type"] == "IRI":
+            return self.env.createNamedNode(triple_fragment["value"])
+        elif triple_fragment["type"] == "blank node":
+            return self._call_state.bnodes[triple_fragment["value"]]
+        elif triple_fragment["type"] == "literal":
             language = None
-            if 'language' in triple_fragment:
-                language = triple_fragment['language']
+            if "language" in triple_fragment:
+                language = triple_fragment["language"]
             return self.env.createLiteral(
-                value=triple_fragment['value'],
-                datatype=self.env.createNamedNode(triple_fragment['datatype']),
-                language=language
+                value=triple_fragment["value"],
+                datatype=self.env.createNamedNode(triple_fragment["datatype"]),
+                language=language,
             )
 
     def process_jobj(self, jobj, options=None):
         from pyld.jsonld import to_rdf
+
         dataset = to_rdf(jobj, options=options)
         for graph_name, triples in dataset.items():
             graph_iri = (
-                self.env.createNamedNode(graph_name) if
-                graph_name != '@default' else
-                None
+                self.env.createNamedNode(graph_name)
+                if graph_name != "@default"
+                else None
             )
             for triple in triples:
                 self.make_quad(
-                    (self.process_triple_fragment(triple['subject']),
-                     self.process_triple_fragment(triple['predicate']),
-                     self.process_triple_fragment(triple['object']),
-                     graph_iri,
-                     )
+                    (
+                        self.process_triple_fragment(triple["subject"]),
+                        self.process_triple_fragment(triple["predicate"]),
+                        self.process_triple_fragment(triple["object"]),
+                        graph_iri,
+                    )
                 )
 
 
 jsonld_parser = PyLDLoader()
```

### Comparing `pymantic-0.3.0/pymantic/parsers/lark/base.py` & `pymantic-1.0.0/src/pymantic/parsers/lark/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from pymantic.compat import (
-    binary_type,
-)
-
-
-class LarkParser(object):
+class LarkParser:
     """Provide a consistent interface for parsing serialized RDF using one
     of the lark parsers.
     """
+
     def __init__(self, lark):
         self.lark = lark
 
     def line_by_line_parser(self, stream):
         for line in stream:  # Equivalent to readline
             if line:
                 yield next(self.lark.parse(line))
@@ -23,28 +19,27 @@
 
         try:
             if graph is None:
                 graph = tf._make_graph()
 
             tf._prepare_parse(graph)
 
-            if hasattr(string_or_stream, 'readline'):
+            if hasattr(string_or_stream, "readline"):
                 triples = self.line_by_line_parser(string_or_stream)
             else:
                 # Presume string.
                 triples = self.lark.parse(string_or_stream)
 
             graph.addAll(triples)
         finally:
             tf._cleanup_parse()
 
         return graph
 
     def parse_string(self, string_or_bytes, graph=None):
-        """Parse a string, decoding it from bytes to UTF-8 if necessary.
-        """
-        if isinstance(string_or_bytes, binary_type):
-            string = string_or_bytes.decode('utf-8')
+        """Parse a string, decoding it from bytes to UTF-8 if necessary."""
+        if isinstance(string_or_bytes, bytes):
+            string = string_or_bytes.decode("utf-8")
         else:
             string = string_or_bytes
 
         return self.parse(string, graph)
```

### Comparing `pymantic-0.3.0/pymantic/parsers/lark/nquads.py` & `pymantic-1.0.0/src/pymantic/parsers/lark/nquads.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,40 +8,35 @@
 
 If ``.parse()`` is called with a file-like object implementing ``readline``,
 it will efficiently parse line by line rather than parsing the entire file.
 """
 
 from lark import Lark
 
-from pymantic.primitives import (
-    Quad,
-)
+from pymantic.primitives import Quad
 
-from .base import (
-    LarkParser,
-)
-from .ntriples import (
-    grammar,
-    NTriplesTransformer,
-)
+from .base import LarkParser
+from .ntriples import NTriplesTransformer, grammar
 
 
 class NQuadsTransformer(NTriplesTransformer):
-    """Transform the tokenized nquads into RDF primitives.
-    """
+    """Transform the tokenized nquads into RDF primitives."""
+
     def quad(self, children):
         subject, predicate, object_, graph = children
         return self.make_quad(subject, predicate, object_, graph)
 
     def quads_start(self, children):
         for child in children:
             if isinstance(child, Quad):
                 yield child
 
 
 nq_lark = Lark(
-    grammar, start='quads_start', parser='lalr',
+    grammar,
+    start="quads_start",
+    parser="lalr",
     transformer=NQuadsTransformer(),
 )
 
-#! A fully-instantiated nquads parser
+# A fully-instantiated nquads parser
 nquads_parser = LarkParser(nq_lark)
```

### Comparing `pymantic-0.3.0/pymantic/parsers/lark/ntriples.py` & `pymantic-1.0.0/src/pymantic/parsers/lark/ntriples.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,21 @@
   graph = ntriples_parser.parse(io.open('a_file.nt', mode='rt'))
   graph2 = ntriples_parser.parse("<http://a.example/s> <http://a.example/p> <http://a.example/o> .")
 
 If ``.parse()`` is called with a file-like object implementing ``readline``,
 it will efficiently parse line by line rather than parsing the entire file.
 """
 
-from lark import (
-    Lark,
-    Transformer,
-)
+from lark import Lark, Transformer
 
-from pymantic.primitives import (
-    NamedNode,
-    Triple,
-)
-from pymantic.util import (
-    decode_literal,
-)
-
-from pymantic.parsers.base import (
-    BaseParser,
-)
-from .base import (
-    LarkParser,
-)
+from pymantic.parsers.base import BaseParser
+from pymantic.primitives import NamedNode, Triple
+from pymantic.util import decode_literal
 
+from .base import LarkParser
 
 grammar = r"""triples_start: triple? (EOL triple)* EOL?
 triple: subject predicate object "."
 
 quads_start: quad? (EOL quad)* EOL?
 quad: subject predicate object graph "."
 
@@ -59,35 +46,35 @@
 HEX: /[0-9A-Fa-f]/
 
 %ignore /[ \t]/+
 """
 
 
 class NTriplesTransformer(BaseParser, Transformer):
-    """Transform the tokenized ntriples into RDF primitives.
-    """
+    """Transform the tokenized ntriples into RDF primitives."""
+
     def blank_node_label(self, children):
-        bn_label, = children
+        (bn_label,) = children
         return self.make_blank_node(bn_label.value)
 
     def iriref(self, children):
-        iri = ''.join(children)
+        iri = "".join(children)
         iri = decode_literal(iri)
         return self.make_named_node(iri)
 
     def literal(self, children):
         quoted_literal = children[0]
 
         quoted_literal = quoted_literal[1:-1]  # Remove ""s
         literal = decode_literal(quoted_literal)
 
         if len(children) == 2 and isinstance(children[1], NamedNode):
             type_ = children[1]
             return self.make_datatype_literal(literal, type_)
-        elif len(children) == 2 and children[1].type == 'LANGTAG':
+        elif len(children) == 2 and children[1].type == "LANGTAG":
             lang = children[1][1:]  # Remove @
             return self.make_language_literal(literal, lang)
         else:
             return self.make_language_literal(literal)
 
     def triple(self, children):
         subject, predicate, object_ = children
@@ -96,13 +83,15 @@
     def triples_start(self, children):
         for child in children:
             if isinstance(child, Triple):
                 yield child
 
 
 nt_lark = Lark(
-    grammar, start='triples_start', parser='lalr',
+    grammar,
+    start="triples_start",
+    parser="lalr",
     transformer=NTriplesTransformer(),
 )
 
-#! A fully-instantiated ntriples parser
+# A fully-instantiated ntriples parser
 ntriples_parser = LarkParser(nt_lark)
```

### Comparing `pymantic-0.3.0/pymantic/parsers/lark/turtle.py` & `pymantic-1.0.0/src/pymantic/parsers/lark/turtle.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,44 +8,21 @@
   p: <http://a.example/p> <http://a.example/o> .\"\"\")
 
 Unlike :mod:`pymantic.parsers.lark.ntriples`, this parser cannot efficiently
 parse turtle line by line. If a file-like object is provided, the entire file
 will be read into memory and parsed there.
 """
 
-from __future__ import unicode_literals
-
+from lark import Lark, Transformer, Tree
+from lark.lexer import Token
 import re
 
-from lark import (
-    Lark,
-    Transformer,
-    Tree,
-)
-from lark.lexer import (
-    Token,
-)
-
-from pymantic.compat import (
-    binary_type,
-)
-from pymantic.parsers.base import (
-    BaseParser,
-)
-from pymantic.primitives import (
-    BlankNode,
-    Literal,
-    NamedNode,
-    Triple,
-)
-from pymantic.util import (
-    grouper,
-    smart_urljoin,
-    decode_literal,
-)
+from pymantic.parsers.base import BaseParser
+from pymantic.primitives import BlankNode, Literal, NamedNode, Triple
+from pymantic.util import decode_literal, grouper, smart_urljoin
 
 RDF_TYPE = NamedNode("http://www.w3.org/1999/02/22-rdf-syntax-ns#type")
 RDF_NIL = NamedNode("http://www.w3.org/1999/02/22-rdf-syntax-ns#nil")
 RDF_FIRST = NamedNode("http://www.w3.org/1999/02/22-rdf-syntax-ns#first")
 RDF_REST = NamedNode("http://www.w3.org/1999/02/22-rdf-syntax-ns#rest")
 
 XSD_DECIMAL = NamedNode("http://www.w3.org/2001/XMLSchema#decimal")
@@ -308,15 +285,15 @@
 def parse(string_or_stream, graph=None, base=""):
     if hasattr(string_or_stream, "readline"):
         string = string_or_stream.read()
     else:
         # Presume string.
         string = string_or_stream
 
-    if isinstance(string_or_stream, binary_type):
+    if isinstance(string_or_stream, bytes):
         string = string_or_stream.decode("utf-8")
     else:
         string = string_or_stream
 
     tree = turtle_lark.parse(string)
     tr = TurtleTransformer(base_iri=base)
     if graph is None:
```

### Comparing `pymantic-0.3.0/pymantic/parsers/rdfxml.py` & `pymantic-1.0.0/src/pymantic/parsers/rdfxml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,85 @@
+from lxml import etree
 import re
 from threading import local
-from urllib.parse import (
-    urljoin,
-)
-
-from lxml import etree
+from urllib.parse import urljoin
 
-from pymantic.primitives import (
-    BlankNode,
-    NamedNode,
-)
+from pymantic.primitives import BlankNode, NamedNode
 
+scheme_re = re.compile(r"[a-zA-Z](?:[a-zA-Z0-9]|\+|-|\.)*")
 
-scheme_re = re.compile(r'[a-zA-Z](?:[a-zA-Z0-9]|\+|-|\.)*')
 
-
-class RDFXMLParser(object):
-    RDF_TYPE = 'http://www.w3.org/1999/02/22-rdf-syntax-ns#type'
+class RDFXMLParser:
+    RDF_TYPE = "http://www.w3.org/1999/02/22-rdf-syntax-ns#type"
 
     def __init__(self):
         self.namespaces = {
-            'rdf': 'http://www.w3.org/1999/02/22-rdf-syntax-ns#',
+            "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
         }
         self._call_state = local()
 
     def clark(self, prefix, tag):
-        return '{%s}%s' % (self.namespaces[prefix], tag)
+        return "{%s}%s" % (self.namespaces[prefix], tag)
 
     def parse(self, f, sink=None):
         self._call_state.bnodes = {}
         tree = etree.parse(f)
-        if tree.getroot() != self.clark('rdf', 'RDF'):
-            raise ValueError('Invalid XML document.')
+        if tree.getroot() != self.clark("rdf", "RDF"):
+            raise ValueError("Invalid XML document.")
         for element in tree.getroot():
             self._handle_resource(element, sink)
 
     def _handle_resource(self, element, sink):
         from pymantic.primitives import NamedNode, Triple
+
         subject = self._determine_subject(element)
-        if element.tag != self.clark('rdf', 'Description'):
+        if element.tag != self.clark("rdf", "Description"):
             resource_class = self._resolve_tag(element)
             sink.add(Triple(subject, NamedNode(self.RDF_TYPE), resource_class))
         for property_element in element:
-            if property_element.tag == self.clark('rdf', 'li'):
+            if property_element.tag == self.clark("rdf", "li"):
                 pass
             else:
                 predicate = self._resolve_tag(property_element)
-            if self.clark('rdf', 'resource') in property_element.attrib:
+            if self.clark("rdf", "resource") in property_element.attrib:
                 object_ = self._resolve_uri(
-                    property_element, property_element.attrib[self.clark(
-                        'rdf', 'resource')])
-                sink.add(
-                    Triple(subject, NamedNode(predicate), NamedNode(object_)))
+                    property_element,
+                    property_element.attrib[self.clark("rdf", "resource")],
+                )
+                sink.add(Triple(subject, NamedNode(predicate), NamedNode(object_)))
         return subject
 
     def _resolve_tag(self, element):
-        if element.tag[0] == '{':
-            tag_bits = element[1:].partition('}')
+        if element.tag[0] == "{":
+            tag_bits = element[1:].partition("}")
             return NamedNode(tag_bits[0] + tag_bits[2])
         else:
             return NamedNode(urljoin(element.base, element.tag))
 
     def _determine_subject(self, element):
-        if self.clark('rdf', 'about') not in element.attrib and\
-           self.clark('rdf', 'nodeID') not in element.attrib and\
-           self.clark('rdf', 'ID') not in element.attrib:
+        if (
+            self.clark("rdf", "about") not in element.attrib
+            and self.clark("rdf", "nodeID") not in element.attrib
+            and self.clark("rdf", "ID") not in element.attrib
+        ):
             return BlankNode()
-        elif self.clark('rdf', 'nodeID') in element.attrib:
-            node_id = element.attrib[self.clark('rdf', 'nodeID')]
+        elif self.clark("rdf", "nodeID") in element.attrib:
+            node_id = element.attrib[self.clark("rdf", "nodeID")]
             if node_id not in self._call_state.bnodes:
                 self._call_state.bnodes[node_id] = BlankNode()
             return self._call_state.bnodes[node_id]
-        elif self.clark('rdf', 'ID') in element.attrib:
+        elif self.clark("rdf", "ID") in element.attrib:
             if not element.base:
-                raise ValueError('No XML base for %r', element)
-            return NamedNode(element.base + '#' +
-                             element.attrib[self.clark('rdf', 'ID')])
-        elif self.clark('rdf', 'about') in element.attrib:
-            return self._resolve_uri(element, element.attrib[
-                self.clark('rdf', 'resource')])
+                raise ValueError("No XML base for %r", element)
+            return NamedNode(
+                element.base + "#" + element.attrib[self.clark("rdf", "ID")]
+            )
+        elif self.clark("rdf", "about") in element.attrib:
+            return self._resolve_uri(
+                element, element.attrib[self.clark("rdf", "resource")]
+            )
 
     def _resolve_uri(self, element, uri):
         if not scheme_re.match(uri):
             return NamedNode(urljoin(element.base, uri))
         else:
             return NamedNode(uri)
```

### Comparing `pymantic-0.3.0/pymantic/primitives.py` & `pymantic-1.0.0/src/pymantic/primitives.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-__all__ = ['Triple', 'Quad', 'q_as_t', 't_as_q', 'Literal', 'NamedNode',
-           'Prefix', 'BlankNode', 'Graph', 'Dataset', 'PrefixMap', 'TermMap',
-           'parse_curie', 'is_language', 'lang_match', 'to_curie', 'Profile',
-           ]
+__all__ = [
+    "Triple",
+    "Quad",
+    "q_as_t",
+    "t_as_q",
+    "Literal",
+    "NamedNode",
+    "Prefix",
+    "BlankNode",
+    "Graph",
+    "Dataset",
+    "PrefixMap",
+    "TermMap",
+    "parse_curie",
+    "is_language",
+    "lang_match",
+    "to_curie",
+    "Profile",
+]
 
 import collections
 from collections import defaultdict
-
 import datetime
 from operator import itemgetter
-from .compat import (
-    text_type,
-    string_types,
-    iteritems,
-    itervalues,
-    iterkeys,
-)
 
+from pymantic.serializers import nt_escape
 import pymantic.uri_schemes as uri_schemes
-
 from pymantic.util import quote_normalized_iri
-from pymantic.serializers import nt_escape
 
 
 def is_language(lang):
     """Is something a valid XML language?"""
     if isinstance(lang, NamedNode):
         return False
     return True
@@ -33,18 +39,19 @@
     """Determines if two languages are, in fact, the same language.
 
     Eg: en is the same as en-us and en-uk."""
     if lang1 is None and lang2 is None:
         return True
     elif lang1 is None or lang2 is None:
         return False
-    lang1 = lang1.partition('-')
-    lang2 = lang2.partition('-')
-    return lang1[0] == lang2[0] and (lang1[2] == '' or lang2[2] == '' or
-                                     lang1[2] == lang2[2])
+    lang1 = lang1.partition("-")
+    lang2 = lang2.partition("-")
+    return lang1[0] == lang2[0] and (
+        lang1[2] == "" or lang2[2] == "" or lang1[2] == lang2[2]
+    )
 
 
 def parse_curie(curie, prefixes):
     """
     Parses a CURIE within the context of the given namespaces. Will also accept
     explicit URIs and wrap them in an rdflib URIRef.
 
@@ -54,30 +61,30 @@
        standard URIs, it is wrapped in a URIRef and returned unchanged.
     2) Otherwise, the CURIE is parsed by the rules of CURIE Syntax 1.0:
        http://www.w3.org/TR/2007/WD-curie-20070307/ The default namespace is
        the namespace keyed by the empty string in the namespaces dictionary.
     3) If the CURIE's namespace cannot be resolved, a ValueError is raised.
     """
     definitely_curie = False
-    if curie[0] == '[' and curie[-1] == ']':
+    if curie[0] == "[" and curie[-1] == "]":
         curie = curie[1:-1]
         definitely_curie = True
-    prefix, sep, reference = curie.partition(':')
+    prefix, sep, reference = curie.partition(":")
     if not definitely_curie:
         if prefix in uri_schemes.schemes:
             return NamedNode(curie)
-    if not reference and '' in prefixes:
+    if not reference and "" in prefixes:
         reference = prefix
-        return Prefix(prefixes[''])(reference)
+        return Prefix(prefixes[""])(reference)
     if prefix in prefixes:
         return Prefix(prefixes[prefix])(reference)
     else:
         raise ValueError(
-            'Could not parse CURIE prefix {} from prefixes {}'.format(
-                prefix, prefixes))
+            f"Could not parse CURIE prefix {prefix} from prefixes {prefixes}"
+        )
 
 
 def parse_curies(curies, namespaces):
     """Parse multiple CURIEs at once."""
     for curie in curies:
         yield parse_curie(curie, namespaces)
 
@@ -96,117 +103,119 @@
     matches = []
     for prefix, namespace in namespaces.items():
         if uri.startswith(namespace):
             matches.append((prefix, namespace))
     if len(matches) > 0:
         prefix, namespace = sorted(matches, key=lambda pair: -len(pair[1]))[0]
         if explicit:
-            return '[' + uri.replace(namespace, prefix + seperator) + ']'
+            return f"[{uri.replace(namespace, prefix + seperator)}]"
         else:
             return uri.replace(namespace, prefix + seperator)
     return uri
 
 
 class Triple(tuple):
     """Triple(subject, predicate, object)
 
     The Triple interface represents an RDF Triple. The stringification of a
     Triple results in an N-Triples.
-        """
+    """
 
     __slots__ = ()
 
-    _fields = ('subject', 'predicate', 'object')
+    _fields = ("subject", "predicate", "object")
 
     def __new__(_cls, subject, predicate, object):
         return tuple.__new__(_cls, (subject, predicate, object))
 
     @classmethod
     def _make(cls, iterable, new=tuple.__new__, len=len):
-        'Make a new Triple object from a sequence or iterable'
+        "Make a new Triple object from a sequence or iterable"
         result = new(cls, iterable)
         if len(result) != 3:
-            raise TypeError('Expected 3 arguments, got %d' % len(result))
+            raise TypeError("Expected 3 arguments, got %d" % len(result))
         return result
 
     def __repr__(self):
-        return 'Triple(subject=%r, predicate=%r, object=%r)' % self
+        return "Triple(subject=%r, predicate=%r, object=%r)" % self
 
     def _asdict(t):
-        'Return a new dict which maps field names to their values'
-        return {'subject': t[0], 'predicate': t[1], 'object': t[2]}
+        "Return a new dict which maps field names to their values"
+        return {"subject": t[0], "predicate": t[1], "object": t[2]}
 
     def _replace(_self, **kwds):
-        'Return a new Triple object replacing specified fields with new values'
-        result = _self._make(map(kwds.pop, ('subject', 'predicate', 'object'),
-                                 _self))
+        "Return a new Triple object replacing specified fields with new values"
+        result = _self._make(map(kwds.pop, ("subject", "predicate", "object"), _self))
         if kwds:
-            raise ValueError('Got unexpected field names: %r' % kwds.keys())
+            raise ValueError("Got unexpected field names: %r" % kwds.keys())
         return result
 
     def __getnewargs__(self):
         return tuple(self)
 
     subject = property(itemgetter(0))
     predicate = property(itemgetter(1))
     object = property(itemgetter(2))
 
     def __str__(self):
-        return self.subject.toNT() + ' ' + self.predicate.toNT() + ' ' + \
-               self.object.toNT() + ' .\n'
+        return f"{self.subject.toNT()} {self.predicate.toNT()} {self.object.toNT()} .\n"
 
     def toString(self):
         return str(self)
 
 
 class Quad(tuple):
-    'Quad(subject, predicate, object, graph)'
+    "Quad(subject, predicate, object, graph)"
 
     __slots__ = ()
 
-    _fields = ('subject', 'predicate', 'object', 'graph')
+    _fields = ("subject", "predicate", "object", "graph")
 
     def __new__(_cls, subject, predicate, object, graph):
         return tuple.__new__(_cls, (subject, predicate, object, graph))
 
     @classmethod
     def _make(cls, iterable, new=tuple.__new__, len=len):
-        'Make a new Quad object from a sequence or iterable'
+        "Make a new Quad object from a sequence or iterable"
         result = new(cls, iterable)
         if len(result) != 4:
-            raise TypeError('Expected 4 arguments, got %d' % len(result))
+            raise TypeError("Expected 4 arguments, got %d" % len(result))
         return result
 
     def __repr__(self):
-        return 'Quad(subject=%r, predicate=%r, object=%r, graph=%r)' % self
+        return "Quad(subject=%r, predicate=%r, object=%r, graph=%r)" % self
 
     def _asdict(t):
-        'Return a new dict which maps field names to their values'
-        return {'subject': t[0], 'predicate': t[1], 'object': t[2],
-                'graph': t[3], }
+        "Return a new dict which maps field names to their values"
+        return {
+            "subject": t[0],
+            "predicate": t[1],
+            "object": t[2],
+            "graph": t[3],
+        }
 
     def _replace(_self, **kwds):
-        'Return a new Quad object replacing specified fields with new values'
-        result = _self._make(map(kwds.pop, ('subject', 'predicate', 'object',
-                                            'graph'), _self))
+        "Return a new Quad object replacing specified fields with new values"
+        result = _self._make(
+            map(kwds.pop, ("subject", "predicate", "object", "graph"), _self)
+        )
         if kwds:
-            raise ValueError('Got unexpected field names: %r' % kwds.keys())
+            raise ValueError("Got unexpected field names: %r" % kwds.keys())
         return result
 
     def __getnewargs__(self):
         return tuple(self)
 
     subject = property(itemgetter(0))
     predicate = property(itemgetter(1))
     object = property(itemgetter(2))
     graph = property(itemgetter(3))
 
     def __str__(self):
-        return str(self.subject) + ' ' + str(self.predicate) + ' ' + \
-               str(self.object) + ' ' + str(self.graph) + ' .\n'
+        return f"{str(self.subject)} {str(self.predicate)} {str(self.object)} {str(self.graph)} .\n"
 
 
 def q_as_t(quad):
     return Triple(quad.subject, quad.predicate, quad.object)
 
 
 def t_as_q(graph_name, triple):
@@ -227,132 +236,132 @@
     attribute specified by a text string token, as specified in [BCP47],
     normalized to lowercase (e.g., 'en', 'fr', 'en-gb').
 
     Literals may not have both a datatype and a language."""
 
     __slots__ = ()
 
-    _fields = ('value', 'language', 'datatype')
+    _fields = ("value", "language", "datatype")
 
     types = {
-        int: lambda v: (str(v), XSD('integer')),
-        datetime.datetime: lambda v: (v.isoformat(), XSD('dateTime'))
+        int: lambda v: (str(v), XSD("integer")),
+        datetime.datetime: lambda v: (v.isoformat(), XSD("dateTime")),
     }
 
     def __new__(_cls, value, language=None, datatype=None):
-        if not isinstance(value, string_types):
+        if not isinstance(value, str):
             value, auto_datatype = _cls.types[type(value)](value)
             if datatype is None:
                 datatype = auto_datatype
         return tuple.__new__(_cls, (value, language, datatype))
 
     @classmethod
     def _make(cls, iterable, new=tuple.__new__, len=len):
-        'Make a new Literal object from a sequence or iterable'
+        "Make a new Literal object from a sequence or iterable"
         result = new(cls, iterable)
         if len(result) != 3:
-            raise TypeError('Expected 3 arguments, got %d' % len(result))
+            raise TypeError("Expected 3 arguments, got %d" % len(result))
         return result
 
     def __repr__(self):
-        return 'Literal(value=%r, language=%r, datatype=%r)' % self
+        return "Literal(value=%r, language=%r, datatype=%r)" % self
 
     def _asdict(t):
-        'Return a new dict which maps field names to their values'
-        return {'value': t[0], 'language': t[1], 'datatype': t[2]}
+        "Return a new dict which maps field names to their values"
+        return {"value": t[0], "language": t[1], "datatype": t[2]}
 
     def _replace(_self, **kwds):
-        'Return a new Literal object replacing specified fields with new value'
-        result = _self._make(map(kwds.pop, ('value', 'language', 'datatype'),
-                                 _self))
+        "Return a new Literal object replacing specified fields with new value"
+        result = _self._make(map(kwds.pop, ("value", "language", "datatype"), _self))
         if kwds:
-            raise ValueError('Got unexpected field names: %r' % kwds.keys())
+            raise ValueError("Got unexpected field names: %r" % kwds.keys())
         return result
 
     def __getnewargs__(self):
         return tuple(self)
 
     value = property(itemgetter(0))
     language = property(itemgetter(1))
     datatype = property(itemgetter(2))
 
     interfaceName = "Literal"
 
     def __str__(self):
-        return text_type(self.value)
+        return str(self.value)
 
     def toNT(self):
         quoted = '"' + nt_escape(self.value) + '"'
         if self.language:
-            return quoted + '@' + self.language
+            return f"{quoted}@{self.language}"
         elif self.datatype:
-            return quoted + '^^' + self.datatype.toNT()
+            return f"{quoted}^^{self.datatype.toNT()}"
         else:
             return quoted
 
 
-class NamedNode(text_type):
+class NamedNode(str):
     """A node identified by an IRI."""
 
     interfaceName = "NamedNode"
 
     @property
     def value(self):
         return self
 
     def __repr__(self):
-        return 'NamedNode(' + self.toNT() + ')'
+        return f"NamedNode({self.toNT()})"
 
     def __str__(self):
         return self.value
 
     def toNT(self):
-        return '<' + nt_escape(quote_normalized_iri(self.value)) + '>'
+        return f"<{nt_escape(quote_normalized_iri(self.value))}>"
 
 
 class Prefix(NamedNode):
     """Node that when called returns the the argument conctantated with
     self."""
+
     def __call__(self, name):
         return NamedNode(self + name)
 
 
 XSD = Prefix("http://www.w3.org/2001/XMLSchema#")
 
 
-class BlankNode(object):
+class BlankNode:
     """A BlankNode is a reference to an unnamed resource (one for which an IRI
     is not known), and may be used in a Triple as a unique reference to that
     unnamed resource.
 
     BlankNodes are stringified by prepending "_:" to a unique value, for
     instance _:b142 or _:me, this stringified form is referred to as a
     "blank node identifier"."""
 
     interfaceName = "BlankNode"
 
     @property
     def value(self):
-        return ''.join(chr(ord(c) + 17) for c in hex(id(self))[2:])
+        return "".join(chr(ord(c) + 17) for c in hex(id(self))[2:])
 
     def __repr__(self):
-        return 'BlankNode()'
+        return "BlankNode()"
 
     def __str__(self):
-        return '_:' + self.value
+        return "_:" + self.value
 
     def toNT(self):
         return str(self)
 
 
 def Index():
     return defaultdict(Index)
 
 
-class Graph(object):
+class Graph:
     """A `Graph` holds a set of one or more `Triple`. Implements the Python
     set/sequence API for `in`, `for`, and `len`"""
 
     def __init__(self, graph_uri=None):
         if not isinstance(graph_uri, NamedNode):
             graph_uri = NamedNode(graph_uri)
         self._uri = graph_uri
@@ -410,41 +419,40 @@
         if subject:
             if predicate:  # s, p, ???
                 if object:  # s, p, o
                     if Triple(subject, predicate, object) in self:
                         yield Triple(subject, predicate, object)
                 else:  # s, p, ?var
                     if subject in self._spo and predicate in self._spo[subject]:
-                        for triple in itervalues(self._spo[subject][predicate]):
+                        for triple in self._spo[subject][predicate].values():
                             yield triple
             else:  # s, ?var, ???
                 if object:  # s, ?var, o
                     if object in self._osp and subject in self._osp[object]:
-                        for triple in itervalues(self._osp[object][subject]):
+                        for triple in self._osp[object][subject].values():
                             yield triple
                 else:  # s, ?var, ?var
                     if subject in self._spo:
                         for predicate in self._spo[subject]:
-                            for triple in \
-                              itervalues(self._spo[subject][predicate]):
+                            for triple in self._spo[subject][predicate].values():
                                 yield triple
         elif predicate:  # ?var, p, ???
             if object:  # ?var, p, o
                 if predicate in self._pos and object in self._pos[predicate]:
-                    for triple in itervalues(self._pos[predicate][object]):
+                    for triple in self._pos[predicate][object].values():
                         yield triple
             else:  # ?var, p, ?var
                 if predicate in self._pos:
                     for object in self._pos[predicate]:
-                        for triple in itervalues(self._pos[predicate][object]):
+                        for triple in self._pos[predicate][object].values():
                             yield triple
         elif object:  # ?var, ?var, o
             if object in self._osp:
                 for subject in self._osp[object]:
-                    for triple in itervalues(self._osp[object][subject]):
+                    for triple in self._osp[object][subject].values():
                         yield triple
         else:
             for triple in self._triples:
                 yield triple
 
     def removeMatches(self, subject, predicate, object):
         """This method removes those triples in the current graph which match
@@ -481,27 +489,26 @@
 
     def toArray(self):
         """Return the set of :py:class:`Triple` within the :py:class:`Graph`"""
         return frozenset(self._triples)
 
     def subjects(self):
         """Returns an iterator over subjects in the graph."""
-        return iterkeys(self._spo)
+        return self._spo.keys()
 
     def predicates(self):
         """Returns an iterator over predicates in the graph."""
-        return iterkeys(self._pos)
+        return self._pos.keys()
 
     def objects(self):
         """Returns an iterator over objects in the graph."""
-        return iterkeys(self._osp)
-
+        return self._osp.keys()
 
-class Dataset(object):
 
+class Dataset:
     def __init__(self):
         self._graphs = defaultdict(Graph)
 
     def add(self, quad):
         self._graphs[quad.graph]._uri = quad.graph
         self._graphs[quad.graph].add(q_as_t(quad))
 
@@ -525,20 +532,19 @@
 
     def match(self, subject=None, predicate=None, object=None, graph=None):
         if graph:
             matches = self._graphs[graph].match(subject, predicate, object)
             for match in matches:
                 yield t_as_q(graph, match)
         else:
-            for graph_uri, graph in iteritems(self._graphs):
+            for graph_uri, graph in self._graphs.items():
                 for match in graph.match(subject, predicate, object):
                     yield t_as_q(graph_uri, match)
 
-    def removeMatches(self, subject=None, predicate=None, object=None,
-                      graph=None):
+    def removeMatches(self, subject=None, predicate=None, object=None, graph=None):
         """This method removes those triples in the current graph which match
         the given arguments."""
         for quad in self.match(subject, predicate, object, graph):
             self.remove(quad)
         return self
 
     def addAll(self, dataset_or_quads):
@@ -553,20 +559,20 @@
 
     def __contains__(self, item):
         if hasattr(item, "graph"):
             if item.graph in self._graphs:
                 graph = self._graphs[item.graph]
                 return q_as_t(item) in graph
         else:
-            for graph in itervalues(self._graphs):
+            for graph in self._graphs.values():
                 if item in graph:
                     return True
 
     def __iter__(self):
-        for graph in itervalues(self._graphs):
+        for graph in self._graphs.values():
             for triple in graph:
                 yield t_as_q(graph.uri, triple)
 
     def toArray(self):
         return frozenset(self)
 
 
@@ -620,80 +626,79 @@
         IRI is returned."""
         return to_curie(iri, self)
 
     def addAll(self, other, override=False):
         if override:
             self.update(other)
         else:
-            for key, value in iteritems(other):
+            for key, value in other.items():
                 if key not in self:
                     self[key] = value
         return self
 
     def setDefault(self, iri):
         """Set the iri to be used when resolving CURIEs without a prefix, for
         example ":this"."""
-        self[''] = iri
+        self[""] = iri
 
 
 class TermMap(dict):
     """A map of simple string terms to IRIs, and provides methods to turn one
-    in to the other.
-
-Example usage:
+        in to the other.
 
->>> terms = TermMap()
+    Example usage:
 
-Create a new term mapping for the term "member"
+    >>> terms = TermMap()
 
->>> terms['member'] = "http://www.w3.org/ns/org#member"
+    Create a new term mapping for the term "member"
 
-Resolve a known term to an IRI
+    >>> terms['member'] = "http://www.w3.org/ns/org#member"
 
->>> terms.resolve("member")
-u"http://www.w3.org/ns/org#member"
+    Resolve a known term to an IRI
 
-Shrink an IRI for a known term to a term
+    >>> terms.resolve("member")
+    u"http://www.w3.org/ns/org#member"
 
->>> terms.shrink("http://www.w3.org/ns/org#member")
-u"member"
+    Shrink an IRI for a known term to a term
 
-Attempt to resolve an unknown term
+    >>> terms.shrink("http://www.w3.org/ns/org#member")
+    u"member"
 
->>> terms.resolve("label")
-None
+    Attempt to resolve an unknown term
 
-Set the default term vocabulary and then attempt to resolve an unknown term
+    >>> terms.resolve("label")
+    None
 
->>> terms.setDefault("http://www.w3.org/2000/01/rdf-schema#")
->>> terms.resolve("label")
-u"http://www.w3.org/2000/01/rdf-schema#label"
+    Set the default term vocabulary and then attempt to resolve an unknown term
 
-"""
+    >>> terms.setDefault("http://www.w3.org/2000/01/rdf-schema#")
+    >>> terms.resolve("label")
+    u"http://www.w3.org/2000/01/rdf-schema#label"
+    """
 
     def addAll(self, other, override=False):
         if override:
             self.update(other)
         else:
-            for key, value in iteritems(other):
+            for key, value in other.items():
                 if key not in self:
                     self[key] = value
         return self
 
     def resolve(self, term):
         """Given a valid term for which an IRI is known (for example "label"),
         this method will return the resulting IRI (for example
         "http://www.w3.org/2000/01/rdf-schema#label").
 
         If no term is known and a default has been set, the IRI is obtained by
         concatenating the term and the default iri.
 
         If no term is known and no default is set, then this method returns
         null."""
-        if hasattr(self, 'default'):
+        if hasattr(self, "default"):
             return self.get(term, self.default + term)
         else:
             return self.get(term)
 
     def setDefault(self, iri):
         """The default iri to be used when an term cannot be resolved, the
         resulting IRI is obtained by concatenating this iri with the term being
@@ -701,43 +706,42 @@
         self.default = iri
 
     def shrink(self, iri):
         """Given an IRI for which an term is known (for example
         "http://www.w3.org/2000/01/rdf-schema#label") this method returns a
         term (for example "label"), if no term is known the original IRI is
         returned."""
-        for term, v in iteritems(self):
+        for term, v in self.items():
             if v == iri:
                 return term
         return iri
 
 
-class Profile(object):
+class Profile:
     """Profiles provide an easy to use context for negotiating between CURIEs,
     Terms and IRIs."""
 
     def __init__(self, prefixes=None, terms=None):
         self.prefixes = prefixes or PrefixMap()
         self.terms = terms or TermMap()
-        if 'rdf' not in self.prefixes:
-            self.prefixes['rdf'] = \
-                'http://www.w3.org/1999/02/22-rdf-syntax-ns#'
-        if 'xsd' not in self.prefixes:
-            self.prefixes['xsd'] = 'http://www.w3.org/2001/XMLSchema#'
+        if "rdf" not in self.prefixes:
+            self.prefixes["rdf"] = "http://www.w3.org/1999/02/22-rdf-syntax-ns#"
+        if "xsd" not in self.prefixes:
+            self.prefixes["xsd"] = "http://www.w3.org/2001/XMLSchema#"
 
     def resolve(self, toresolve):
         """Given an Term or CURIE this method will return an IRI, or null if it
         cannot be resolved.
 
         If toresolve contains a : (colon) then this method returns the result
         of calling prefixes.resolve(toresolve)
 
         otherwise this method returns the result of calling
         terms.resolve(toresolve)"""
-        if ':' in toresolve:
+        if ":" in toresolve:
             return self.prefixes.resolve(toresolve)
         else:
             return self.terms.resolve(toresolve)
 
     def setDefaultVocabulary(self, iri):
         """This method sets the default vocabulary for use when resolving
         unknown terms, it is identical to calling the setDefault method on
@@ -771,14 +775,15 @@
         self.terms.addAll(profile.terms, override)
         return self
 
 
 class RDFEnvironment(Profile):
     """The RDF Environment is an interface which exposes a high level API for
     working with RDF in a programming environment."""
+
     def createBlankNode(self):
         """Creates a new :py:class:`BlankNode`."""
         return BlankNode()
 
     def createNamedNode(self, value):
         """Creates a new :py:class:`NamedNode`."""
         return NamedNode(value)
@@ -800,15 +805,15 @@
         allows easy transition between native sequences and Graphs and is the
         counterpart for :py:meth:`Graph.toArray`."""
         g = Graph()
         g.addAll(triples)
         return g
 
     def createAction(self, test, action):
-        raise NotImplemented
+        raise NotImplementedError()
 
     def createProfile(self, empty=False):
         if empty:
             return Profile()
         else:
             return Profile(self.prefixes, self.terms)
```

### Comparing `pymantic-0.3.0/pymantic/rdf.py` & `pymantic-1.0.0/src/pymantic/rdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 """Provides common classes and functions for modelling an RDF graph using
 Python objects."""
 
-import os.path
-from .compat.moves.urllib import parse as urlparse
-import re
 import logging
-from .compat.moves import cStringIO as StringIO
-from string import Template
 
-import pymantic.util as util
-from pymantic.primitives import *
-from .compat import (
-    add_metaclass,
-    string_types,
-    text_type,
+from pymantic.primitives import (
+    BlankNode,
+    Literal,
+    NamedNode,
+    Prefix,
+    PrefixMap,
+    Profile,
+    Triple,
+    is_language,
+    lang_match,
+    parse_curie,
 )
+import pymantic.util as util
 
 log = logging.getLogger(__name__)
 
+
 class MetaResource(type):
     """Aggregates Prefix and scalar information."""
 
-    _classes = {} # Map of RDF classes to Python classes.
+    _classes = {}  # Map of RDF classes to Python classes.
 
     def __new__(cls, name, bases, dct):
         prefixes = PrefixMap()
         scalars = set()
         for base in bases:
-            if hasattr(base, 'prefixes'):
+            if hasattr(base, "prefixes"):
                 prefixes.update(base.prefixes)
-            if hasattr(base, 'scalars'):
+            if hasattr(base, "scalars"):
                 scalars.update(base.scalars)
-        if 'prefixes' in dct:
-            for prefix in dct['prefixes']:
-                prefixes[prefix] = Prefix(dct['prefixes'][prefix])
-        dct['prefixes'] = prefixes
-        if 'scalars' in dct:
-            for scalar in dct['scalars']:
+        if "prefixes" in dct:
+            for prefix in dct["prefixes"]:
+                prefixes[prefix] = Prefix(dct["prefixes"][prefix])
+        dct["prefixes"] = prefixes
+        if "scalars" in dct:
+            for scalar in dct["scalars"]:
                 scalars.add(parse_curie(scalar, prefixes))
-        dct['scalars'] = frozenset(scalars)
-        dct['_meta_resource'] = cls
+        dct["scalars"] = frozenset(scalars)
+        dct["_meta_resource"] = cls
 
         return type.__new__(cls, name, bases, dct)
 
+
 def register_class(rdf_type):
     """Register a class for automatic instantiation VIA Resource.classify."""
+
     def _register_class(python_class):
-        rdf_class = python_class.resolve(rdf_type)
         MetaResource._classes[python_class.resolve(rdf_type)] = python_class
         python_class.rdf_classes = frozenset((python_class.resolve(rdf_type),))
         return python_class
+
     return _register_class
 
+
 class URLRetrievalError(Exception):
     """Raised when an attempt to retrieve a resource returns a status other
     than 200 OK."""
+
     pass
 
 
-@add_metaclass(MetaResource)
-class Resource(object):
+class Resource(metaclass=MetaResource):
     """Provides necessary context and utility methods for accessing a Resource
     in an RDF graph. Resources can be used as-is, but are likely somewhat
     unwieldy, since all predicate access must be by complete URL and produces
     sets. By subclassing Resource, you can take advantage of a number of
     quality-of-life features:
 
     1) Bind prefixes to prefixes, and refer to them using CURIEs when
@@ -94,133 +99,152 @@
        calling Resource.classify. You can also create a new instance of a
        Resource by calling .new on a subclass.
 
     Automatic retrieval of resources with no type information is currently
     implemented here, but is likely to be refactored into a separate persistence
     layer in the near future."""
 
-    prefixes = {'rdf': 'http://www.w3.org/1999/02/22-rdf-syntax-ns#',
-                  'rdfs': 'http://www.w3.org/2000/01/rdf-schema#'}
+    prefixes = {
+        "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+        "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+    }
 
-    scalars = frozenset(('rdfs:label',))
+    scalars = frozenset(("rdfs:label",))
 
-    lang = 'en'
+    lang = "en"
 
     rdf_classes = frozenset()
 
     global_profile = Profile()
 
     def __init__(self, graph, subject):
         self.graph = graph
         if not isinstance(subject, NamedNode) and not isinstance(subject, BlankNode):
             subject = NamedNode(subject)
         self.subject = subject
 
     @classmethod
-    def new(cls, graph, subject = None):
+    def new(cls, graph, subject=None):
         """Add type information to the graph for a new instance of this Resource."""
-        #for prefix, Prefix in cls.prefixes.iteritems():
-            #graph.bind(prefix, Prefix)
+        # for prefix, Prefix in cls.prefixes.iteritems():
+        # graph.bind(prefix, Prefix)
         if subject is None:
             subject = BlankNode()
         if not isinstance(subject, NamedNode):
             subject = NamedNode(subject)
         for rdf_class in cls.rdf_classes:
-            graph.add(Triple(subject, cls.resolve('rdf:type'), rdf_class))
+            graph.add(Triple(subject, cls.resolve("rdf:type"), rdf_class))
         return cls(graph, subject)
 
     def erase(self):
         """Erase all tripes for this resource from the graph."""
         for triple in list(self.graph.match(self.subject, None, None)):
             self.graph.remove(triple)
 
     def is_a(self):
         """Test to see if the subject of this resource has all the necessary
         RDF classes applied to it."""
-        if hasattr(self, 'rdf_classes'):
+        if hasattr(self, "rdf_classes"):
             for rdf_class in self.rdf_classes:
-                if not any(self.graph.match(self.subject,
-                                                   self.resolve('rdf:type'),
-                                                   rdf_class)):
+                if not any(
+                    self.graph.match(self.subject, self.resolve("rdf:type"), rdf_class)
+                ):
                     return False
         return True
 
     @classmethod
     def resolve(cls, key):
         """Use this class's prefixes to resolve a curie"""
         try:
             return cls.prefixes.resolve(key)
         except ValueError:
             return cls.global_profile.resolve(key)
 
     def __eq__(self, other):
         if isinstance(other, Resource):
             return self.subject == other.subject
-        elif isinstance(other, NamedNode) or isinstance(other, string_types):
-            return text_type(self.subject) == text_type(other)
+        elif isinstance(other, NamedNode) or isinstance(other, str):
+            return str(self.subject) == str(other)
         return NotImplemented
 
     def __ne__(self, other):
         eq = self.__eq__(other)
         if eq is NotImplemented:
             return NotImplemented
         else:
             return not eq
 
     def __hash__(self):
         return hash(self.subject)
 
     def bare_literals(self, predicate):
         """Objects for a predicate that are language-less, datatype-less Literals."""
-        return [t.object for t in self.graph.match(self.subject, predicate, None) if\
-                hasattr(t.object, 'language') and t.object.language is None and\
-                hasattr(t.object, 'datatype') and t.object.datatype is None]
+        return [
+            t.object
+            for t in self.graph.match(self.subject, predicate, None)
+            if hasattr(t.object, "language")
+            and t.object.language is None
+            and hasattr(t.object, "datatype")
+            and t.object.datatype is None
+        ]
 
     def objects_by_lang(self, predicate, lang=None):
         """Objects for a predicate that match a specified language or, if
         language is None, have a language specified."""
         if lang:
-            return [t.object for t in self.graph.match(self.subject, predicate, None) if\
-                    hasattr(t.object, 'language') and lang_match(lang, t.object.language)]
-        elif lang == '':
+            return [
+                t.object
+                for t in self.graph.match(self.subject, predicate, None)
+                if hasattr(t.object, "language") and lang_match(lang, t.object.language)
+            ]
+        elif lang == "":
             return self.bare_literals(predicate)
         else:
-            return [t.object for t in self.graph.match(self.subject, predicate, None) if\
-                    hasattr(t.object, 'language') and t.object.language is not None]
+            return [
+                t.object
+                for t in self.graph.match(self.subject, predicate, None)
+                if hasattr(t.object, "language") and t.object.language is not None
+            ]
 
     def objects_by_datatype(self, predicate, datatype=None):
         """Objects for a predicate that match a specified datatype or, if
         datatype is None, have a datatype specified."""
         if datatype:
-            return [t.object for t in self.graph.match(self.subject, predicate, None) if\
-                    hasattr(t.object, 'datatype') and t.object.datatype == datatype]
-        elif datatype == '':
+            return [
+                t.object
+                for t in self.graph.match(self.subject, predicate, None)
+                if hasattr(t.object, "datatype") and t.object.datatype == datatype
+            ]
+        elif datatype == "":
             return self.bare_literals(predicate)
         else:
-            return [t.object for t in self.graph.match(self.subject, predicate, None) if\
-                    hasattr(t.object, 'datatype') and t.object.datatype is not None]
+            return [
+                t.object
+                for t in self.graph.match(self.subject, predicate, None)
+                if hasattr(t.object, "datatype") and t.object.datatype is not None
+            ]
 
-    def objects_by_type(self, predicate, resource_class = None):
+    def objects_by_type(self, predicate, resource_class=None):
         """Objects for a predicate that are instances of a particular Resource
         subclass or, if resource_class is none, are Resources."""
         selected_objects = []
         for t in self.graph.match(self.subject, predicate, None):
             obj = t.object
             if isinstance(obj, BlankNode) or isinstance(obj, NamedNode):
-                if resource_class is None or\
-                   isinstance(self.classify(self.graph, obj),
-                              resource_class):
+                if resource_class is None or isinstance(
+                    self.classify(self.graph, obj), resource_class
+                ):
                     selected_objects.append(obj)
         return selected_objects
 
     def objects(self, predicate):
         """All objects for a predicate."""
         return [t.object for t in self.graph.match(self.subject, predicate, None)]
 
-    def object_of(self, predicate = None):
+    def object_of(self, predicate=None):
         """All subjects for which this resource is an object for the given
         predicate."""
         if predicate is None:
             for triple in self.graph.match(None, None, self.subject):
                 yield (self.classify(self.graph, triple.subject), triple.predicate)
         else:
             predicate = self.resolve(predicate)
@@ -240,17 +264,19 @@
 
         resource['rdfs:label', 'en']
 
         Passing in a value of None will result in all values for the predicate
         in question being returned."""
         predicate, objects = self._objects_for_key(key)
         if predicate not in self.scalars or (isinstance(key, tuple) and key[1] is None):
+
             def getitem_iter_results():
                 for obj in objects:
                     yield self.classify(self.graph, obj)
+
             return getitem_iter_results()
         else:
             return self.classify(self.graph, util.one_or_none(objects))
 
     def get_scalar(self, key):
         """As __getitem__ access, but pretend the key is a scalar even if it isn't.
 
@@ -285,16 +311,17 @@
         predicate, lang, datatype, rdf_class = self._interpret_key(key)
         value = literalize(self.graph, value, lang, datatype)
         if not isinstance(key, tuple):
             # Implicit specification.
             objects = self._objects_for_implicit_set(predicate, value)
         else:
             # Explicit specification.
-            objects = self._objects_for_explicit_set(predicate, value, lang,
-                                                     datatype, rdf_class)
+            objects = self._objects_for_explicit_set(
+                predicate, value, lang, datatype, rdf_class
+            )
         for obj in objects:
             self.graph.remove(Triple(self.subject, predicate, obj))
         if isinstance(value, frozenset):
             for obj in value:
                 if isinstance(obj, Resource):
                     self.graph.add(Triple(self.subject, predicate, obj.subject))
                 else:
@@ -334,71 +361,85 @@
 
     @classmethod
     def in_graph(cls, graph):
         """Iterate through all instances of this Resource in the graph."""
         subjects = set()
         for rdf_class in cls.rdf_classes:
             if not subjects:
-                subjects.update([t.subject for t in graph.match(
-                    None, cls.resolve('rdf:type'), rdf_class)])
+                subjects.update(
+                    [
+                        t.subject
+                        for t in graph.match(None, cls.resolve("rdf:type"), rdf_class)
+                    ]
+                )
             else:
-                subjects.intersection_update([t.subject for t in graph.match(
-                    None, cls.resolve('rdf:type'), rdf_class)])
+                subjects.intersection_update(
+                    [
+                        t.subject
+                        for t in graph.match(None, cls.resolve("rdf:type"), rdf_class)
+                    ]
+                )
         return set(cls(graph, subject) for subject in subjects)
 
     def __repr__(self):
         return "<%r: %s>" % (type(self), self.subject)
 
     def __str__(self):
-        if self['rdfs:label']:
-            return self['rdfs:label'].value
+        if self["rdfs:label"]:
+            return self["rdfs:label"].value
         else:
             return str(self.subject)
 
     @classmethod
     def classify(cls, graph, obj):
         """Classify an object into an appropriate registered class, or Resource.
 
         May create a new class if necessary that is a subclass of two or more
         registered Resource classes."""
         if obj is None:
             return None
         if isinstance(obj, Literal):
             return obj
-        if any(graph.match(obj, cls.resolve('rdf:type'), None)):
-            #retrieve_resource(graph, obj)
-            if not any(graph.match(obj, cls.resolve('rdf:type'), None)):
+        if any(graph.match(obj, cls.resolve("rdf:type"), None)):
+            # retrieve_resource(graph, obj)
+            if not any(graph.match(obj, cls.resolve("rdf:type"), None)):
                 return Resource(graph, obj)
-        types = frozenset([t.object for t in graph.match(
-            obj, cls.resolve('rdf:type'), None)])
-        python_classes = tuple(cls._meta_resource._classes[t] for t in types if\
-                               t in cls._meta_resource._classes)
+        types = frozenset(
+            [t.object for t in graph.match(obj, cls.resolve("rdf:type"), None)]
+        )
+        python_classes = tuple(
+            cls._meta_resource._classes[t]
+            for t in types
+            if t in cls._meta_resource._classes
+        )
         if len(python_classes) == 0:
             return Resource(graph, obj)
         elif len(python_classes) == 1:
             return python_classes[0](graph, obj)
         else:
             if types not in cls._meta_resource._classes:
                 the_class = cls._meta_resource.__new__(
-                    cls._meta_resource, ''.join(python_class.__name__ for\
-                                               python_class in python_classes),
-                    python_classes, {'_autocreate': True})
+                    cls._meta_resource,
+                    "".join(python_class.__name__ for python_class in python_classes),
+                    python_classes,
+                    {"_autocreate": True},
+                )
                 cls._meta_resource._classes[types] = the_class
                 the_class.rdf_classes = frozenset(types)
             return cls._meta_resource._classes[types](graph, obj)
 
     def _interpret_key(self, key):
         """Break up a key into a predicate name and optional language or
         datatype specifier."""
         lang = None
         datatype = None
         rdf_class = None
         if isinstance(key, tuple) and len(key) >= 2:
             if key[1] is None:
-                pass # All values are already None, do nothing.
+                pass  # All values are already None, do nothing.
             elif isinstance(key[1], MetaResource):
                 rdf_class = key[1]
             elif is_language(key[1]):
                 lang = key[1]
             else:
                 datatype = self._interpret_datatype(key[1])
             predicate = self.resolve(key[0])
@@ -406,22 +447,21 @@
             predicate = self.resolve(key)
         if not isinstance(key, tuple) and predicate in self.scalars:
             lang = self.lang
         return predicate, lang, datatype, rdf_class
 
     def _interpret_datatype(self, datatype):
         """Deal with xsd:string vs. plain literal"""
-        if datatype == '':
-            return ''
-        elif datatype == 'http://www.w3.org/2001/XMLSchema#string':
-            return ''
+        if datatype == "":
+            return ""
+        elif datatype == "http://www.w3.org/2001/XMLSchema#string":
+            return ""
         else:
             return datatype
 
-
     def _objects_for_key(self, key):
         """Find objects that are potentially interesting when doing normal
         dictionary key-style access - IE, __getitem__, __delitem__, __contains__,
         and pretty much everything but __setitem__."""
         predicate, lang, datatype, rdf_class = self._interpret_key(key)
         # log.debug("predicate: %r lang: %r datatype: %r rdf_class: %r", predicate, lang, datatype, rdf_class)
         if lang is None and datatype is None and rdf_class is None:
@@ -438,124 +478,145 @@
                 objects += self.objects_by_type(predicate)
         elif datatype:
             objects = self.objects_by_datatype(predicate, datatype)
             if predicate not in self.scalars:
                 objects += self.objects_by_type(predicate)
         elif rdf_class:
             objects = self.objects_by_type(predicate, rdf_class)
-        elif lang == '' or datatype == '':
+        elif lang == "" or datatype == "":
             objects = self.bare_literals(predicate)
         else:
-            raise KeyError('Invalid key: ' + repr(key))
+            raise KeyError("Invalid key: " + repr(key))
         return predicate, objects
 
     def _objects_for_implicit_set(self, predicate, value):
         """Find the objects that should be removed from the graph when doing a
         dictionary-style set with implicit type information."""
-        if (isinstance(value, frozenset) or (isinstance(value, tuple) and\
-                                             not isinstance(value, Literal))) and\
-           predicate in self.scalars:
-            raise ValueError('Cannot store sequences in scalars')
-        elif predicate in self.scalars and isinstance(value, Literal)\
-             and value.language:
-            return self.objects_by_lang(predicate, value.language) +\
-                   self.objects_by_datatype(predicate) +\
-                   self.objects_by_type(predicate) +\
-                   self.bare_literals(predicate)
+        if (
+            isinstance(value, frozenset)
+            or (isinstance(value, tuple) and not isinstance(value, Literal))
+        ) and predicate in self.scalars:
+            raise ValueError("Cannot store sequences in scalars")
+        elif (
+            predicate in self.scalars and isinstance(value, Literal) and value.language
+        ):
+            return (
+                self.objects_by_lang(predicate, value.language)
+                + self.objects_by_datatype(predicate)
+                + self.objects_by_type(predicate)
+                + self.bare_literals(predicate)
+            )
         else:
             return self.objects(predicate)
 
     def _objects_for_explicit_set(self, predicate, value, lang, datatype, rdf_class):
         """Find the objects that should be removed from the graph when doing a
         dictionary-style set with explicit type information."""
         if not check_objects(self.graph, value, lang, datatype, rdf_class):
-            raise ValueError('Improper value provided.')
+            raise ValueError("Improper value provided.")
         if lang and predicate in self.scalars:
-            return self.objects_by_lang(predicate, lang) +\
-                   self.objects_by_datatype(predicate) +\
-                   self.objects_by_type(predicate)
+            return (
+                self.objects_by_lang(predicate, lang)
+                + self.objects_by_datatype(predicate)
+                + self.objects_by_type(predicate)
+            )
         elif lang and predicate not in self.scalars:
-            return self.objects_by_lang(predicate, lang) +\
-                   self.objects_by_type(predicate)
+            return self.objects_by_lang(predicate, lang) + self.objects_by_type(
+                predicate
+            )
         elif predicate in self.scalars:
             return self.objects(predicate)
         elif datatype:
-            return self.objects_by_datatype(predicate, datatype) +\
-                   self.objects_by_type(predicate)
+            return self.objects_by_datatype(predicate, datatype) + self.objects_by_type(
+                predicate
+            )
         elif rdf_class:
             return self.objects_by_type(predicate, rdf_class)
 
     def copy(self, target_subject):
         """Create copies of all triples with this resource as their subject
         with the target subject as their subject. Returns a classified version
         of the target subject."""
-        if not isinstance(target_subject, NamedNode) and\
-           not isinstance(target_subject, BlankNode):
+        if not isinstance(target_subject, NamedNode) and not isinstance(
+            target_subject, BlankNode
+        ):
             target_subject = NamedNode(target_subject)
         for t in self.graph.match(self.subject, None, None):
             self.graph.add((target_subject, t.predicate, t.object))
         return self.classify(self.graph, target_subject)
 
     def as_(self, target_class):
         return target_class(self.graph, self.subject)
 
 
 class List(Resource):
     """Convenience class for dealing with RDF lists.
 
     Requires considerable use of ``as_``, due to the utter lack of type
     information on said lists."""
-    scalars = frozenset(('rdf:first', 'rdf:rest'))
+
+    scalars = frozenset(("rdf:first", "rdf:rest"))
 
     def __iter__(self):
         """Iterating over lists works differently from normal Resources."""
         current = self
-        while current.subject != self.resolve('rdf:nil'):
-            yield current['rdf:first']
-            current = current['rdf:rest']
-            if current.subject != self.resolve('rdf:nil'):
+        while current.subject != self.resolve("rdf:nil"):
+            yield current["rdf:first"]
+            current = current["rdf:rest"]
+            if current.subject != self.resolve("rdf:nil"):
                 current = current.as_(type(self))
 
     @classmethod
     def is_list(cls, node, graph):
         """Determine if a given node is plausibly the subject of a list element."""
-        return bool(list(graph.match(
-            subject = node, predicate = cls.resolve('rdf:rest'))))
+        return bool(list(graph.match(subject=node, predicate=cls.resolve("rdf:rest"))))
 
 
 def literalize(graph, value, lang, datatype):
     """Convert either a value or a sequence of values to either a Literal or
     a Resource."""
-    if isinstance(value, set) or isinstance(value, frozenset) or\
-       isinstance(value, list) or (isinstance(value, tuple) and\
-                                   not isinstance(value, Literal)):
+    if (
+        isinstance(value, set)
+        or isinstance(value, frozenset)
+        or isinstance(value, list)
+        or (isinstance(value, tuple) and not isinstance(value, Literal))
+    ):
         return frozenset(objectify_value(graph, v, lang, datatype) for v in value)
     else:
         return objectify_value(graph, value, lang, datatype)
 
-def objectify_value(graph, value, lang = None, datatype = None):
+
+def objectify_value(graph, value, lang=None, datatype=None):
     """Convert a single value into either a Literal or a Resource."""
     if isinstance(value, BlankNode) or isinstance(value, NamedNode):
         return Resource.classify(graph, value)
     elif isinstance(value, Literal) or isinstance(value, Resource):
         return value
-    elif isinstance(value, string_types):
-        return Literal(value, language = lang, datatype = datatype)
+    elif isinstance(value, str):
+        return Literal(value, language=lang, datatype=datatype)
     else:
         return Literal(value)
 
+
 def check_objects(graph, value, lang, datatype, rdf_class):
     """Determine that value or the things in values are appropriate for the
     specified explicit object access key."""
-    if isinstance(value, frozenset) or (isinstance(value, tuple) and\
-                                        not isinstance(value, Literal)):
+    if isinstance(value, frozenset) or (
+        isinstance(value, tuple) and not isinstance(value, Literal)
+    ):
         for v in value:
-            if (lang and (not hasattr(v, 'language') or\
-                          not lang_match(v.language, lang))) or \
-               (datatype and v.datatype != datatype) or \
-               (rdf_class and not isinstance(v, rdf_class)):
+            if (
+                (
+                    lang
+                    and (not hasattr(v, "language") or not lang_match(v.language, lang))
+                )
+                or (datatype and v.datatype != datatype)
+                or (rdf_class and not isinstance(v, rdf_class))
+            ):
                 return False
         return True
     else:
-        return (lang and lang_match(value.language, lang)) or \
-               (datatype and value.datatype == datatype) or \
-               (rdf_class and isinstance(value, rdf_class))
+        return (
+            (lang and lang_match(value.language, lang))
+            or (datatype and value.datatype == datatype)
+            or (rdf_class and isinstance(value, rdf_class))
+        )
```

### Comparing `pymantic-0.3.0/pymantic/serializers.py` & `pymantic-1.0.0/src/pymantic/serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,169 @@
 from collections import OrderedDict
 
-import re
-import warnings
-from .compat import (
-    iteritems,
-    text_type,
-)
 
 def nt_escape(node_string):
     """Properly escape strings for n-triples and n-quads serialization."""
-    output_string = ''
+    output_string = ""
     for char in node_string:
-        if char == u'\u0009':
-            output_string += '\\t'
-        elif char == u'\u000A':
-            output_string += '\\n'
-        elif char == u'\u000D':
-            output_string += '\\r'
-        elif char == u'\u0022':
+        if char == "\u0009":
+            output_string += "\\t"
+        elif char == "\u000A":
+            output_string += "\\n"
+        elif char == "\u000D":
+            output_string += "\\r"
+        elif char == "\u0022":
             output_string += '\\"'
-        elif char == u'\u005C':
-            output_string += '\\\\'
-        elif char >= u'\u0020' and char <= u'\u0021' or\
-             char >= u'\u0023' and char <= u'\u005B' or\
-             char >= u'\u005D' and char <= u'\u007E':
+        elif char == "\u005C":
+            output_string += "\\\\"
+        elif (
+            char >= "\u0020"
+            and char <= "\u0021"
+            or char >= "\u0023"
+            and char <= "\u005B"
+            or char >= "\u005D"
+            and char <= "\u007E"
+        ):
             output_string += char
-        elif char >= u'\u007F' and char <= u'\uFFFF':
-            output_string += '\\u%04X' % ord(char)
-        elif char >= u'\U00010000' and char <= u'\U0010FFFF':
-            output_string += '\\U%08X' % ord(char)
+        elif char >= "\u007F" and char <= "\uFFFF":
+            output_string += "\\u%04X" % ord(char)
+        elif char >= "\U00010000" and char <= "\U0010FFFF":
+            output_string += "\\U%08X" % ord(char)
     return output_string
 
+
 def serialize_ntriples(graph, f):
     """Serialize some graph to f as ntriples."""
     for triple in graph:
         f.write(str(triple))
 
+
 def serialize_nquads(dataset, f):
     """Serialize some graph to f as nquads."""
     for quad in dataset:
         f.write(str(quad))
 
+
 def default_bnode_name_generator():
     i = 0
     while True:
-        yield '_b' + str(i)
+        yield "_b" + str(i)
         i += 1
 
+
 def escape_prefix_local(prefix):
-    prefix, colon, local = prefix.partition(':')
+    prefix, colon, local = prefix.partition(":")
     for esc_char in "~.-!$&'()*+,;=:/?#@%_":
-        local = local.replace(esc_char, '\\' + esc_char)
-    return ''.join((prefix,colon,local))
+        local = local.replace(esc_char, "\\" + esc_char)
+    return "".join((prefix, colon, local))
+
 
 def turtle_string_escape(string):
     """Escape a string appropriately for output in turtle form."""
     from pymantic.util import ECHAR_MAP
 
-    for escaped, value in iteritems(ECHAR_MAP):
-        string = string.replace(value, '\\' + escaped)
+    for escaped, value in ECHAR_MAP.items():
+        string = string.replace(value, "\\" + escaped)
     return '"' + string + '"'
 
+
 def turtle_repr(node, profile, name_map, bnode_name_maker, base=None):
     """Turn a node in an RDF graph into its turtle representation."""
-    if node.interfaceName == 'NamedNode':
+    if node.interfaceName == "NamedNode":
         name = profile.prefixes.shrink(node)
         if base and name.startswith(base):
             if base.endswith("#"):
-                name = '<' + text_type(name.replace(base, "#")) + '>'
+                name = f"<{str(name.replace(base, '#'))}>"
             else:
-                name = '<' + text_type(name.replace(base, "")) + '>'
+                name = f"<{str(name.replace(base, ''))}>"
         if name == node:
-            name = '<' + text_type(name) + '>'
+            name = f"<{str(name)}>"
         else:
             escape_prefix_local(name)
-    elif node.interfaceName == 'BlankNode':
+    elif node.interfaceName == "BlankNode":
         if node in name_map:
             name = name_map[node]
         else:
             name = bnode_name_maker.next()
             name_map[node] = name
-    elif node.interfaceName == 'Literal':
-        if node.datatype == profile.resolve('xsd:string'):
+    elif node.interfaceName == "Literal":
+        if node.datatype == profile.resolve("xsd:string"):
             # Simple string.
             name = turtle_string_escape(node.value)
-        elif node.datatype == None:
+        elif node.datatype is None:
             # String with language?
             name = turtle_string_escape(node.value)
             if node.language:
-                name += '@' + node.language
-        elif node.datatype == profile.resolve('xsd:integer'):
+                name += "@" + node.language
+        elif node.datatype == profile.resolve("xsd:integer"):
             name = node.value
-        elif node.datatype == profile.resolve('xsd:decimal'):
+        elif node.datatype == profile.resolve("xsd:decimal"):
             name = node.value
-        elif node.datatype == profile.resolve('xsd:double'):
+        elif node.datatype == profile.resolve("xsd:double"):
             name = node.value
-        elif node.datatype == profile.resolve('xsd:boolean'):
+        elif node.datatype == profile.resolve("xsd:boolean"):
             name = node.value
         else:
             # Unrecognized data-type.
             name = turtle_string_escape(node.value)
-            name += '^' + turtle_repr(node.datatype, profile, None, None)
+            name += "^" + turtle_repr(node.datatype, profile, None, None)
     return name
 
-def turtle_sorted_names(l, name_maker):
+
+def turtle_sorted_names(nodes, name_maker):
     """Sort a list of nodes in a graph by turtle name."""
-    return sorted((name_maker(n), n) for n in l)
+    return sorted((name_maker(node), node) for node in nodes)
 
-def serialize_turtle(graph, f, base=None, profile=None,
-                     bnode_name_generator=default_bnode_name_generator):
+
+def serialize_turtle(
+    graph, f, base=None, profile=None, bnode_name_generator=default_bnode_name_generator
+):
     """Serialize a graph to f as turtle, optionally using base IRI base
     and prefix map from profile. If provided, subject_key will be used to order
     subjects, and predicate_key predicates within a subject."""
 
     if base is not None:
-        f.write('@base <' + base + '> .\n')
+        f.write("@base <" + base + "> .\n")
     if profile is None:
         from pymantic.primitives import Profile
+
         profile = Profile()
-    for prefix, iri in iteritems(profile.prefixes):
-        if prefix != 'rdf':
-            f.write('@prefix ' + prefix + ': <' + iri + '> .\n')
+    for prefix, iri in profile.prefixes.items():
+        if prefix != "rdf":
+            f.write("@prefix " + prefix + ": <" + iri + "> .\n")
 
     name_map = OrderedDict()
-    output_order = []
     bnode_name_maker = bnode_name_generator()
 
-    name_maker = lambda n: turtle_repr(n, profile, name_map, bnode_name_maker, base)
+    def name_maker(n):
+        return turtle_repr(n, profile, name_map, bnode_name_maker, base)
 
     from pymantic.rdf import List
 
     subjects = [subj for subj in graph.subjects() if not List.is_list(subj, graph)]
 
     for subject_name, subject in turtle_sorted_names(subjects, name_maker):
         subj_indent_size = len(subject_name) + 1
-        f.write(subject_name + ' ')
-        predicates = set(t.predicate for t in graph.match(subject = subject))
+        f.write(subject_name + " ")
+        predicates = set(t.predicate for t in graph.match(subject=subject))
         sorted_predicates = turtle_sorted_names(predicates, name_maker)
         for i, (predicate_name, predicate) in enumerate(sorted_predicates):
             if i != 0:
-                f.write(' ' * subj_indent_size)
+                f.write(" " * subj_indent_size)
             pred_indent_size = subj_indent_size + len(predicate_name) + 1
-            f.write(predicate_name + ' ')
-            for j, triple in enumerate(graph.match(subject = subject,
-                                                   predicate = predicate)):
+            f.write(predicate_name + " ")
+            for j, triple in enumerate(
+                graph.match(subject=subject, predicate=predicate)
+            ):
                 if j != 0:
-                    f.write(',\n' + ' ' * pred_indent_size)
+                    f.write(",\n" + " " * pred_indent_size)
                 if List.is_list(triple.object, graph):
-                    f.write('(')
+                    f.write("(")
                     for k, o in enumerate(List(graph, triple.object)):
                         if k != 0:
-                            f.write(' ')
+                            f.write(" ")
                         f.write(name_maker(o))
-                    f.write(')')
+                    f.write(")")
                 else:
                     f.write(name_maker(triple.object))
-            f.write(' ;\n')
-        f.write(' ' * subj_indent_size + '.\n\n')
+            f.write(" ;\n")
+        f.write(" " * subj_indent_size + ".\n\n")
```

### Comparing `pymantic-0.3.0/pymantic/sparql.py` & `pymantic-1.0.0/src/pymantic/sparql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """Provide an interface to SPARQL query endpoints."""
 
-from .compat.moves import cStringIO as StringIO
 import datetime
-import urllib
-from .compat.moves.urllib import parse as urlparse
-
+from io import StringIO
+import json
+import logging
 from lxml import objectify
 import pytz
 import rdflib
 import requests
-import json
-
-import logging
+import urllib
+from urllib.parse import urlparse
 
 log = logging.getLogger(__name__)
 
 
 class SPARQLQueryException(Exception):
 
     """Raised when the SPARQL store returns an HTTP status code other than 200 OK."""
@@ -26,27 +24,29 @@
 class UnknownSPARQLReturnTypeException(Exception):
 
     """Raised when the SPARQL store provides a response with an unrecognized content-type."""
 
     pass
 
 
-class _SelectOrUpdate(object):
+class _SelectOrUpdate:
 
     """A server that can run SPARQL queries."""
 
-    def __init__(self, server, sparql, default_graph=None, named_graph=None, *args, **kwargs):
+    def __init__(
+        self, server, sparql, default_graph=None, named_graph=None, *args, **kwargs
+    ):
         self.server = server
         self.sparql = sparql
         self.default_graphs = default_graph
         self.named_graphs = named_graph
         self.headers = dict()
         self.params = dict()
 
-# abstract methods, see Select for the idea
+    # abstract methods, see Select for the idea
     def default_graph_uri(self):
         pass
 
     def named_graph_uri(self):
         pass
 
     def query_or_update(self):
@@ -57,140 +57,149 @@
 
     def postQueries(self):
         pass
 
     def execute(self):
         log.debug("Querying: %s with: %r", self.server.query_url, self.sparql)
 
-        sparql = self.sparql.encode('utf-8')
+        sparql = self.sparql.encode("utf-8")
 
         if self.default_graphs:
             self.params[self.default_graph_uri()] = self.default_graphs
         if self.named_graphs:
             self.params[self.named_graph_uri()] = self.named_graphs
 
         if self.server.post_directly:
             self.headers["Content-Type"] = self.directContentType() + "; charset=utf-8"
             uri_params = self.params
             data = sparql
-            method = 'post'
+            method = "post"
         elif self.postQueries():
             uri_params = None
             self.params[self.query_or_update()] = sparql
             data = self.params
-            method = 'post'
+            method = "post"
         else:
             # select only
             self.params[self.query_or_update()] = sparql
             uri_params = self.params
             data = None
-            method = 'get'
+            method = "get"
 
         response = self.server.s.request(
-            method, self.server.query_url,
-            params=uri_params, headers=self.headers, data=data,
-            **self.server.requests_kwargs)
+            method,
+            self.server.query_url,
+            params=uri_params,
+            headers=self.headers,
+            data=data,
+            **self.server.requests_kwargs
+        )
         if response.status_code == 204:
             return True
         if response.status_code != 200:
-            raise SPARQLQueryException('%s: %s\nQuery: %s' %
-                                       (response.headers, response.content, self.sparql))
+            raise SPARQLQueryException(
+                "%s: %s\nQuery: %s" % (response.headers, response.content, self.sparql)
+            )
         return response
 
 
 class _Select(_SelectOrUpdate):
-
     acceptable_xml_responses = [
-        'application/rdf+xml',
-        'application/sparql-results+xml',
+        "application/rdf+xml",
+        "application/sparql-results+xml",
     ]
 
     acceptable_json_responses = [
-        'application/sparql-results+json',
-        'text/turtle',
+        "application/sparql-results+json",
+        "text/turtle",
     ]
 
-    def __init__(self, server, query, output='json', *args, **kwargs):
+    def __init__(self, server, query, output="json", *args, **kwargs):
         super(_Select, self).__init__(server, query, *args, **kwargs)
-        if output == 'xml':
-            self.headers['Accept'] = ','.join(self.acceptable_xml_responses)
+        if output == "xml":
+            self.headers["Accept"] = ",".join(self.acceptable_xml_responses)
         else:
-            self.headers['Accept'] = ','.join(self.acceptable_json_responses)
+            self.headers["Accept"] = ",".join(self.acceptable_json_responses)
 
     def default_graph_uri(self):
-        return 'default-graph-uri'
+        return "default-graph-uri"
 
     def named_graph_uri(self):
-        return 'named-graph-uri'
+        return "named-graph-uri"
 
     def query_or_update(self):
-        return 'query'
+        return "query"
 
     def directContentType(self):
-        return 'application/sparql-query'
+        return "application/sparql-query"
 
     def postQueries(self):
         return self.server.post_queries
 
     def execute(self):
         response = super(_Select, self).execute()
         format = None
-        if response.headers['content-type'].startswith('application/rdf+xml'):
-            format = 'xml'
-        elif response.headers['content-type'].startswith('text/turtle'):
-            format = 'turtle'
+        if response.headers["content-type"].startswith("application/rdf+xml"):
+            format = "xml"
+        elif response.headers["content-type"].startswith("text/turtle"):
+            format = "turtle"
 
         if format:
             graph = rdflib.ConjunctiveGraph()
             graph.parse(StringIO(response.content), self.query_url, format=format)
             return graph
-        elif response.headers['content-type'].startswith('application/sparql-results+json'):
+        elif response.headers["content-type"].startswith(
+            "application/sparql-results+json"
+        ):
             return json.loads(response.content.decode("utf-8"))
-        elif response.headers['content-type'].startswith('application/sparql-results+xml'):
+        elif response.headers["content-type"].startswith(
+            "application/sparql-results+xml"
+        ):
             return objectify.parse(StringIO(response.content))
         else:
-            raise UnknownSPARQLReturnTypeException('Got content of type: %s' %
-                                                   response.headers['content-type'])
+            raise UnknownSPARQLReturnTypeException(
+                "Got content of type: %s" % response.headers["content-type"]
+            )
 
 
 class _Update(_SelectOrUpdate):
     def default_graph_uri(self):
-        return 'using-graph-uri'
+        return "using-graph-uri"
 
     def named_graph_uri(self):
-        return 'using-named-graph-uri'
+        return "using-named-graph-uri"
 
     def query_or_update(self):
-        return 'update'
+        return "update"
 
     def directContentType(self):
-        return 'application/sparql-update'
+        return "application/sparql-update"
 
     def postQueries(self):
         return True
 
 
-class SPARQLServer(object):
+class SPARQLServer:
 
     """A server that can run SPARQL queries."""
 
     def __init__(self, query_url, post_queries=False, post_directly=False, verify=None):
         self.query_url = query_url
         self.post_queries = post_queries
         self.post_directly = post_directly
         self.requests_kwargs = {}
         if verify is not None:
-            self.requests_kwargs = {'verify': verify}
+            self.requests_kwargs = {"verify": verify}
 
         self.s = requests.Session()
 
     acceptable_sparql_responses = [
-        'application/sparql-results+json',
-        'application/rdf+xml',
-        'application/sparql-results+xml',
+        "application/sparql-results+json",
+        "application/rdf+xml",
+        "application/sparql-results+xml",
     ]
 
     def query(self, sparql, *args, **kwargs):
         """Execute a SPARQL query.
 
         The return type varies based on what the SPARQL store responds with:
 
@@ -217,106 +226,135 @@
 
     def __init__(self, query_url, dataset_url, param_style=True, **kwargs):
         super(UpdateableGraphStore, self).__init__(query_url, **kwargs)
         self.dataset_url = dataset_url
         self.param_style = param_style
 
     acceptable_graph_responses = [
-        'text/plain',
-        'application/rdf+xml',
-        'text/turtle',
-        'text/rdf+n3',
+        "text/plain",
+        "application/rdf+xml",
+        "text/turtle",
+        "text/rdf+n3",
     ]
 
     def request_url(self, graph_uri):
         if self.param_style:
-            return self.dataset_url + '?' + urllib.urlencode({'graph': graph_uri})
+            return self.dataset_url + "?" + urllib.urlencode({"graph": graph_uri})
         else:
             return urlparse.urljoin(self.dataset_url, urllib.quote_plus(graph_uri))
 
     def get(self, graph_uri):
-        response = self.s.get(self.request_url(graph_uri),
-                              headers={'Accept': ','.join(self.acceptable_graph_responses)},
-                              **self.server.requests_kwargs)
+        response = self.s.get(
+            self.request_url(graph_uri),
+            headers={"Accept": ",".join(self.acceptable_graph_responses)},
+            **self.server.requests_kwargs
+        )
         if response.status_code != 200:
-            raise Exception('Error from Graph Store (%s): %s' %
-                            (response.status_code, response.content))
+            raise Exception(
+                "Error from Graph Store (%s): %s"
+                % (response.status_code, response.content)
+            )
         graph = rdflib.ConjunctiveGraph()
-        if response.headers['content-type'].startswith('text/plain'):
-            graph.parse(StringIO(response.content), publicID=graph_uri, format='nt')
-        elif response.headers['content-type'].startswith('application/rdf+xml'):
-            graph.parse(StringIO(response.content), publicID=graph_uri, format='xml')
-        elif response.headers['content-type'].startswith('text/turtle'):
-            graph.parse(StringIO(response.content), publicID=graph_uri, format='turtle')
-        elif response.headers['content-type'].startswith('text/rdf+n3'):
-            graph.parse(StringIO(response.content), publicID=graph_uri, format='n3')
+        if response.headers["content-type"].startswith("text/plain"):
+            graph.parse(StringIO(response.content), publicID=graph_uri, format="nt")
+        elif response.headers["content-type"].startswith("application/rdf+xml"):
+            graph.parse(StringIO(response.content), publicID=graph_uri, format="xml")
+        elif response.headers["content-type"].startswith("text/turtle"):
+            graph.parse(StringIO(response.content), publicID=graph_uri, format="turtle")
+        elif response.headers["content-type"].startswith("text/rdf+n3"):
+            graph.parse(StringIO(response.content), publicID=graph_uri, format="n3")
         return graph
 
     def delete(self, graph_uri):
-        response = self.s.delete(self.request_url(graph_uri),
-                                 **self.server.request_kwargs)
+        response = self.s.delete(
+            self.request_url(graph_uri), **self.server.request_kwargs
+        )
         if response.status_code not in (200, 202):
-            raise Exception('Error from Graph Store (%s): %s' %
-                            (response.status_code, response.content))
+            raise Exception(
+                "Error from Graph Store (%s): %s"
+                % (response.status_code, response.content)
+            )
 
     def put(self, graph_uri, graph):
-        graph_triples = graph.serialize(format='nt')
-        response = self.s.put(self.request_url(graph_uri),
-                              data=graph_triples,
-                              headers={'content-type': 'text/plain'},
-                              **self.server.requests_kwargs)
+        graph_triples = graph.serialize(format="nt")
+        response = self.s.put(
+            self.request_url(graph_uri),
+            data=graph_triples,
+            headers={"content-type": "text/plain"},
+            **self.server.requests_kwargs
+        )
         if response.status_code not in (200, 201, 204):
-            raise Exception('Error from Graph Store (%s): %s' %
-                            (response.status_code, response.content))
+            raise Exception(
+                "Error from Graph Store (%s): %s"
+                % (response.status_code, response.content)
+            )
 
     def post(self, graph_uri, graph):
-        graph_triples = graph.serialize(format='nt')
+        graph_triples = graph.serialize(format="nt")
         if graph_uri is not None:
-            response = self.s.post(self.request_url(graph_uri),
-                                   data=graph_triples,
-                                   headers={'content-type': 'text/plain'},
-                                   **self.server.requests_kwargs)
+            response = self.s.post(
+                self.request_url(graph_uri),
+                data=graph_triples,
+                headers={"content-type": "text/plain"},
+                **self.server.requests_kwargs
+            )
             if response.status_code not in (200, 201, 204):
-                raise Exception('Error from Graph Store (%s): %s' %
-                                (response.status_code, response.content))
+                raise Exception(
+                    "Error from Graph Store (%s): %s"
+                    % (response.status_code, response.content)
+                )
         else:
-            response = self.s.post(self.dataset_url,
-                                   data=graph_triples,
-                                   headers={'content-type': 'text/plain'},
-                                   **self.server.requests_kwargs)
+            response = self.s.post(
+                self.dataset_url,
+                data=graph_triples,
+                headers={"content-type": "text/plain"},
+                **self.server.requests_kwargs
+            )
             if response.status_code != 201:
-                raise Exception('Error from Graph Store (%s): %s' %
-                                (response.status_code, response.content))
+                raise Exception(
+                    "Error from Graph Store (%s): %s"
+                    % (response.status_code, response.content)
+                )
 
 
 class PatchableGraphStore(UpdateableGraphStore):
 
     """A graph store that supports the optional PATCH method of updating RDF graphs."""
 
     def patch(self, graph_uri, changeset):
-        graph_xml = changeset.serialize(format='xml', encoding='utf-8')
-        response = self.s.patch(self.request_url(graph_uri), data=graph_xml,
-                                headers={'content-type': 'application/vnd.talis.changeset+xml'},
-                                **self.server.requests_kwargs)
+        graph_xml = changeset.serialize(format="xml", encoding="utf-8")
+        response = self.s.patch(
+            self.request_url(graph_uri),
+            data=graph_xml,
+            headers={"content-type": "application/vnd.talis.changeset+xml"},
+            **self.server.requests_kwargs
+        )
         if response.status_code not in (200, 201, 204):
-            raise Exception('Error from Graph Store (%s): %s' %
-                            (response.status_code, response.content))
+            raise Exception(
+                "Error from Graph Store (%s): %s"
+                % (response.status_code, response.content)
+            )
         return True
 
 
 def changeset(a, b, graph_uri):
     """Create an RDF graph with the changeset between graphs a and b."""
     cs = rdflib.Namespace("http://purl.org/vocab/changeset/schema#")
     graph = rdflib.Graph()
     graph.namespace_manager.bind("cs", cs)
     removal, addition = differences(a, b)
     change_set = rdflib.BNode()
     graph.add((change_set, rdflib.RDF.type, cs["ChangeSet"]))
-    graph.add((change_set, cs["createdDate"],
-               rdflib.Literal(datetime.datetime.now(pytz.UTC).isoformat())))
+    graph.add(
+        (
+            change_set,
+            cs["createdDate"],
+            rdflib.Literal(datetime.datetime.now(pytz.UTC).isoformat()),
+        )
+    )
     graph.add((change_set, cs["subjectOfChange"], rdflib.URIRef(graph_uri)))
 
     for stmt in removal:
         statement = reify(graph, stmt)
         graph.add((change_set, cs["removal"], statement))
     for stmt in addition:
         statement = reify(graph, stmt)
@@ -334,9 +372,11 @@
     graph.add((statement_node, rdflib.RDF.object, o))
     return statement_node
 
 
 def differences(a, b, exclude=[]):
     """Return (removes,adds) excluding statements with a predicate in exclude."""
     exclude = [rdflib.URIRef(excluded) for excluded in exclude]
-    return ([s for s in a if s not in b and s[1] not in exclude],
-            [s for s in b if s not in a and s[1] not in exclude])
+    return (
+        [s for s in a if s not in b and s[1] not in exclude],
+        [s for s in b if s not in a and s[1] not in exclude],
+    )
```

### Comparing `pymantic-0.3.0/pymantic/tests/test_RDF.py` & `pymantic-1.0.0/tests/test_RDF.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,738 +1,948 @@
 import datetime
-import unittest
+import pytest
 
+from pymantic.primitives import Graph, Literal, NamedNode, Prefix, Triple
 import pymantic.rdf
 import pymantic.util
-from pymantic.primitives import *
-from pymantic.compat import add_metaclass
 
-XSD = Prefix('http://www.w3.org/2001/XMLSchema#')
+XSD = Prefix("http://www.w3.org/2001/XMLSchema#")
 
 RDF = Prefix("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
 
-class TestRDF(unittest.TestCase):
-    def tearDown(self):
-        pymantic.rdf.MetaResource._classes = {}
-
-    def testCurieURI(self):
-        """Test CURIE parsing of explicit URIs."""
-        test_ns = {'http': Prefix('WRONG!'),
-                   'urn': Prefix('WRONG!'),}
-        self.assertEqual(pymantic.rdf.parse_curie('http://oreilly.com', test_ns),
-                         NamedNode('http://oreilly.com'))
-        self.assertEqual(pymantic.rdf.parse_curie('urn:isbn:1234567890123', test_ns),
-                         NamedNode('urn:isbn:1234567890123'))
-
-    def testCurieDefaultPrefix(self):
-        """Test CURIE parsing of CURIEs in the default Prefix."""
-        test_ns = {'': Prefix('foo/'),
-                   'wrong': Prefix('WRONG!')}
-        self.assertEqual(pymantic.rdf.parse_curie('bar', test_ns),
-                         NamedNode('foo/bar'))
-        self.assertEqual(pymantic.rdf.parse_curie('[bar]', test_ns),
-                         NamedNode('foo/bar'))
-        self.assertEqual(pymantic.rdf.parse_curie('baz', test_ns),
-                         NamedNode('foo/baz'))
-        self.assertEqual(pymantic.rdf.parse_curie('[aap]', test_ns),
-                         NamedNode('foo/aap'))
-
-    def testCurieprefixes(self):
-        """Test CURIE parsing of CURIEs in non-default prefixes."""
-        test_ns = {'': Prefix('WRONG!'),
-                   'foo': Prefix('foobly/'),
-                   'bar': Prefix('bardle/'),
-                   'http': Prefix('reallybadidea/'),}
-        self.assertEqual(pymantic.rdf.parse_curie('foo:aap', test_ns),
-                         NamedNode('foobly/aap'))
-        self.assertEqual(pymantic.rdf.parse_curie('[bar:aap]', test_ns),
-                         NamedNode('bardle/aap'))
-        self.assertEqual(pymantic.rdf.parse_curie('[foo:baz]', test_ns),
-                         NamedNode('foobly/baz'))
-        self.assertEqual(pymantic.rdf.parse_curie('bar:baz', test_ns),
-                         NamedNode('bardle/baz'))
-        self.assertEqual(pymantic.rdf.parse_curie('[http://oreilly.com]', test_ns),
-                         NamedNode('reallybadidea///oreilly.com'))
 
-    def testCurieNoSuffix(self):
-        """Test CURIE parsing of CURIEs with no suffix."""
+@pytest.fixture()
+def reset_metaresource():
+    yield
+    pymantic.rdf.MetaResource._classes = {}
+
+
+def testCurieURI(reset_metaresource):
+    """Test CURIE parsing of explicit URIs."""
+    test_ns = {
+        "http": Prefix("WRONG!"),
+        "urn": Prefix("WRONG!"),
+    }
+    assert pymantic.rdf.parse_curie("http://example.com", test_ns) == NamedNode(
+        "http://example.com"
+    )
+    assert pymantic.rdf.parse_curie("urn:isbn:1234567890123", test_ns) == NamedNode(
+        "urn:isbn:1234567890123"
+    )
+
+
+def testCurieDefaultPrefix(reset_metaresource):
+    """Test CURIE parsing of CURIEs in the default Prefix."""
+    test_ns = {"": Prefix("foo/"), "wrong": Prefix("WRONG!")}
+    assert pymantic.rdf.parse_curie("bar", test_ns) == NamedNode("foo/bar")
+    assert pymantic.rdf.parse_curie("[bar]", test_ns) == NamedNode("foo/bar")
+    assert pymantic.rdf.parse_curie("baz", test_ns) == NamedNode("foo/baz")
+    assert pymantic.rdf.parse_curie("[aap]", test_ns) == NamedNode("foo/aap")
+
+
+def testCurieprefixes(reset_metaresource):
+    """Test CURIE parsing of CURIEs in non-default prefixes."""
+    test_ns = {
+        "": Prefix("WRONG!"),
+        "foo": Prefix("foobly/"),
+        "bar": Prefix("bardle/"),
+        "http": Prefix("reallybadidea/"),
+    }
+    assert pymantic.rdf.parse_curie("foo:aap", test_ns) == NamedNode("foobly/aap")
+    assert pymantic.rdf.parse_curie("[bar:aap]", test_ns) == NamedNode("bardle/aap")
+    assert pymantic.rdf.parse_curie("[foo:baz]", test_ns) == NamedNode("foobly/baz")
+    assert pymantic.rdf.parse_curie("bar:baz", test_ns) == NamedNode("bardle/baz")
+    assert pymantic.rdf.parse_curie("[http://example.com]", test_ns) == NamedNode(
+        "reallybadidea///example.com"
+    )
+
+
+def testUnparseableCuries(reset_metaresource):
+    """Test some CURIEs that shouldn't parse."""
+    test_ns = {
+        "foo": Prefix("WRONG!"),
+    }
+    with pytest.raises(ValueError):
+        pymantic.rdf.parse_curie("[bar]", test_ns)
+    with pytest.raises(ValueError):
+        pymantic.rdf.parse_curie("bar", test_ns)
+    with pytest.raises(ValueError):
+        pymantic.rdf.parse_curie("bar:baz", test_ns)
+    with pytest.raises(ValueError):
+        pymantic.rdf.parse_curie("[bar:baz]", test_ns)
+
+
+def testMetaResourceNothingUseful(reset_metaresource):
+    """Test applying a MetaResource to a class without anything it uses."""
+
+    class Foo(metaclass=pymantic.rdf.MetaResource):
         pass
 
-    def testUnparseableCuries(self):
-        """Test some CURIEs that shouldn't parse."""
-        test_ns = {'foo': Prefix('WRONG!'),}
-        self.assertRaises(ValueError, pymantic.rdf.parse_curie, '[bar]', test_ns)
-        self.assertRaises(ValueError, pymantic.rdf.parse_curie, 'bar', test_ns)
-        self.assertRaises(ValueError, pymantic.rdf.parse_curie, 'bar:baz', test_ns)
-        self.assertRaises(ValueError, pymantic.rdf.parse_curie, '[bar:baz]', test_ns)
-
-    def testMetaResourceNothingUseful(self):
-        """Test applying a MetaResource to a class without anything it uses."""
-
-        @add_metaclass(pymantic.rdf.MetaResource)
-        class Foo(object):
-            pass
-
-    def testMetaResourceprefixes(self):
-        """Test the handling of prefixes by MetaResource."""
-
-        @add_metaclass(pymantic.rdf.MetaResource)
-        class Foo(object):
-            prefixes = {'foo': 'bar', 'baz': 'garply', 'meme': 'lolcatz!',}
-
-        self.assertEqual(Foo.prefixes, {'foo': Prefix('bar'),
-                                          'baz': Prefix('garply'),
-                                          'meme': Prefix('lolcatz!'),})
-
-    def testMetaResourcePrefixInheritance(self):
-        """Test the composition of Prefix dictionaries by MetaResource."""
-
-        @add_metaclass(pymantic.rdf.MetaResource)
-        class Foo(object):
-            prefixes = {'foo': 'bar', 'baz': 'garply', 'meme': 'lolcatz!',}
-        class Bar(Foo):
-            prefixes = {'allyourbase': 'arebelongtous!', 'bunny': 'pancake',}
-        self.assertEqual(Foo.prefixes, {'foo': Prefix('bar'),
-                                          'baz': Prefix('garply'),
-                                          'meme': Prefix('lolcatz!'),})
-        self.assertEqual(Bar.prefixes, {'foo': Prefix('bar'),
-                                          'baz': Prefix('garply'),
-                                          'meme': Prefix('lolcatz!'),
-                                          'allyourbase': Prefix('arebelongtous!'),
-                                          'bunny': Prefix('pancake'),})
-
-    def testMetaResourcePrefixInheritanceReplacement(self):
-        """Test the composition of Prefix dictionaries by MetaResource where
-        some prefixes on the parent get replaced."""
-
-        @add_metaclass(pymantic.rdf.MetaResource)
-        class Foo(object):
-            prefixes = {'foo': 'bar', 'baz': 'garply', 'meme': 'lolcatz!',}
-        class Bar(Foo):
-            prefixes = {'allyourbase': 'arebelongtous!', 'bunny': 'pancake',
-                          'foo': 'notbar', 'baz': 'notgarply',}
-        self.assertEqual(Foo.prefixes, {'foo': Prefix('bar'),
-                                          'baz': Prefix('garply'),
-                                          'meme': Prefix('lolcatz!'),})
-        self.assertEqual(Bar.prefixes, {'foo': Prefix('notbar'),
-                                          'baz': Prefix('notgarply'),
-                                          'meme': Prefix('lolcatz!'),
-                                          'allyourbase': Prefix('arebelongtous!'),
-                                          'bunny': Prefix('pancake'),})
-
-    def testResourceEquality(self):
-        graph = Graph()
-        otherGraph = Graph()
-        testResource = pymantic.rdf.Resource(graph, 'foo')
-        self.assertEqual(testResource, pymantic.rdf.Resource(
-            graph, 'foo'))
-        self.assertEqual(testResource, NamedNode('foo'))
-        self.assertEqual(testResource, 'foo')
-        self.assertNotEqual(testResource, pymantic.rdf.Resource(
-            graph, 'bar'))
-        self.assertEqual(testResource, pymantic.rdf.Resource(
-            otherGraph, 'foo'))
-        self.assertNotEqual(testResource, NamedNode('bar'))
-        self.assertNotEqual(testResource, 'bar')
-        self.assertNotEqual(testResource, 42)
-
-    def testClassification(self):
-        """Test classification of a resource."""
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        test_subject = NamedNode('http://example.com/athing')
-        graph = Graph()
-        graph.add(Triple(test_subject, Offering.resolve('rdf:type'),
-                         Offering.resolve('gr:Offering')))
-        offering = pymantic.rdf.Resource.classify(graph, test_subject)
-        self.assert_(isinstance(offering, Offering))
-
-    def testMulticlassClassification(self):
-        """Test classification of a resource that matches multiple registered
-        classes."""
-        @pymantic.rdf.register_class('foaf:Organization')
-        class Organization(pymantic.rdf.Resource):
-            prefixes = {
-                'foaf': 'http://xmlns.com/foaf/0.1/',
-            }
-
-        @pymantic.rdf.register_class('foaf:Group')
-        class Group(pymantic.rdf.Resource):
-            prefixes = {
-                'foaf': 'http://xmlns.com/foaf/0.1/',
-            }
-
-        test_subject1 = NamedNode('http://example.com/aorganization')
-        test_subject2 = NamedNode('http://example.com/agroup')
-        test_subject3 = NamedNode('http://example.com/aorgandgroup')
-        graph = Graph()
-        graph.add(Triple(test_subject1, Organization.resolve('rdf:type'),
-                         Organization.resolve('foaf:Organization')))
-        graph.add(Triple(test_subject2, Group.resolve('rdf:type'),
-                         Group.resolve('foaf:Group')))
-        graph.add(Triple(test_subject3, Organization.resolve('rdf:type'),
-                         Organization.resolve('foaf:Organization')))
-        graph.add(Triple(test_subject3, Organization.resolve('rdf:type'),
-                         Organization.resolve('foaf:Group')))
-        organization = pymantic.rdf.Resource.classify(graph, test_subject1)
-        group = pymantic.rdf.Resource.classify(graph, test_subject2)
-        both = pymantic.rdf.Resource.classify(graph, test_subject3)
-        self.assert_(isinstance(organization, Organization))
-        self.assertFalse(isinstance(organization, Group))
-        self.assertFalse(isinstance(group, Organization))
-        self.assert_(isinstance(group, Group))
-        self.assert_(isinstance(both, Organization))
-        self.assert_(isinstance(both, Group))
-
-    def testStr(self):
-        """Test str-y serialization of Resources."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/aorganization')
-        test_label = Literal('Test Label', language='en')
-        graph.add(Triple(test_subject1,
-                         pymantic.rdf.Resource.resolve('rdfs:label'),
-                         test_label))
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        self.assertEqual(r['rdfs:label'], test_label)
-        self.assertEqual(str(r), test_label.value)
-
-    def testGetSetDelPredicate(self):
-        """Test getting, setting, and deleting a multi-value predicate."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        r['rdfs:example'] = set(('foo', 'bar'))
-        example_values = set(r['rdfs:example'])
-        self.assert_(Literal('foo') in example_values)
-        self.assert_(Literal('bar') in example_values)
-        self.assertEqual(len(example_values), 2)
-        del r['rdfs:example']
-        example_values = set(r['rdfs:example'])
-        self.assertEqual(len(example_values), 0)
-
-    def testGetSetDelScalarPredicate(self):
-        """Test getting, setting, and deleting a scalar predicate."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        r['rdfs:label'] = 'foo'
-        self.assertEqual(r['rdfs:label'], Literal('foo', language='en'))
-        del r['rdfs:label']
-        self.assertEqual(r['rdfs:label'], None)
-
-    def testGetSetDelPredicateLanguage(self):
-        """Test getting, setting and deleting a multi-value predicate with an explicit language."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        r['rdfs:example', 'en'] = set(('baz',))
-        r['rdfs:example', 'fr'] = set(('foo', 'bar'))
-        example_values = set(r['rdfs:example', 'fr'])
-        self.assert_(Literal('foo', language='fr') in example_values)
-        self.assert_(Literal('bar', language='fr') in example_values)
-        self.assert_(Literal('baz', language='en') not in example_values)
-        self.assertEqual(len(example_values), 2)
-        example_values = set(r['rdfs:example', 'en'])
-        self.assert_(Literal('foo', language='fr') not in example_values)
-        self.assert_(Literal('bar', language='fr') not in example_values)
-        self.assert_(Literal('baz', language='en') in example_values)
-        self.assertEqual(len(example_values), 1)
-        del r['rdfs:example', 'fr']
-        example_values = set(r['rdfs:example', 'fr'])
-        self.assertEqual(len(example_values), 0)
-        example_values = set(r['rdfs:example', 'en'])
-        self.assert_(Literal('foo', language='fr') not in example_values)
-        self.assert_(Literal('bar', language='fr') not in example_values)
-        self.assert_(Literal('baz', language='en') in example_values)
-        self.assertEqual(len(example_values), 1)
-
-    def testGetSetDelScalarPredicateLanguage(self):
-        """Test getting, setting, and deleting a scalar predicate with an explicit language."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        r['rdfs:label'] = 'foo'
-        r['rdfs:label', 'fr'] = 'bar'
-        self.assertEqual(r['rdfs:label'], Literal('foo', language='en'))
-        self.assertEqual(r['rdfs:label', 'en'], Literal('foo', language='en'))
-        self.assertEqual(r['rdfs:label', 'fr'], Literal('bar', language='fr'))
-        del r['rdfs:label']
-        self.assertEqual(r['rdfs:label'], None)
-        self.assertEqual(r['rdfs:label', 'en'], None)
-        self.assertEqual(r['rdfs:label', 'fr'], Literal('bar', language='fr'))
-
-    def testGetSetDelPredicateDatatype(self):
-        """Test getting, setting and deleting a multi-value predicate with an explicit datatype."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        now = datetime.datetime.now()
-        then = datetime.datetime.now() - datetime.timedelta(days=1)
-        number = 42
-        r['rdfs:example', XSD('integer')] = set((number,))
-        r['rdfs:example', XSD('dateTime')] = set((now, then,))
-        example_values = set(r['rdfs:example', XSD('dateTime')])
-        self.assert_(Literal(now) in example_values)
-        self.assert_(Literal(then) in example_values)
-        self.assert_(Literal(number) not in example_values)
-        self.assertEqual(len(example_values), 2)
-        example_values = set(r['rdfs:example', XSD('integer')])
-        self.assert_(Literal(now) not in example_values)
-        self.assert_(Literal(then) not in example_values)
-        self.assert_(Literal(number) in example_values)
-        self.assertEqual(len(example_values), 1)
-        del r['rdfs:example', XSD('dateTime')]
-        example_values = set(r['rdfs:example', XSD('dateTime')])
-        self.assertEqual(len(example_values), 0)
-        example_values = set(r['rdfs:example', XSD('integer')])
-        self.assert_(Literal(now) not in example_values)
-        self.assert_(Literal(then) not in example_values)
-        self.assert_(Literal(number) in example_values)
-        self.assertEqual(len(example_values), 1)
-
-    def testGetSetDelScalarPredicateDatatype(self):
-        """Test getting, setting, and deleting a scalar predicate with an explicit datatype."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        now = datetime.datetime.now()
-        number = 42
-        r['rdfs:label', XSD('integer')] = number
-        self.assertEqual(r['rdfs:label', XSD('integer')],
-                         Literal(number, datatype=XSD('integer')))
-        self.assertEqual(r['rdfs:label', XSD('dateTime')], None)
-        self.assertEqual(r['rdfs:label'],
-                         Literal(number, datatype=XSD('integer')))
-        r['rdfs:label', XSD('dateTime')] = now
-        self.assertEqual(r['rdfs:label', XSD('dateTime')], Literal(now))
-        self.assertEqual(r['rdfs:label', XSD('integer')], None)
-        self.assertEqual(r['rdfs:label'], Literal(now))
-        del r['rdfs:label', XSD('integer')]
-        self.assertEqual(r['rdfs:label', XSD('dateTime')], Literal(now))
-        self.assertEqual(r['rdfs:label', XSD('integer')], None)
-        self.assertEqual(r['rdfs:label'], Literal(now))
-        del r['rdfs:label', XSD('dateTime')]
-        self.assertEqual(r['rdfs:label'], None)
-        r['rdfs:label', XSD('integer')] = number
-        self.assertEqual(r['rdfs:label', XSD('integer')],
-                         Literal(number, datatype=XSD('integer')))
-        self.assertEqual(r['rdfs:label', XSD('dateTime')], None)
-        self.assertEqual(r['rdfs:label'], Literal(number, datatype=XSD('integer')))
-        del r['rdfs:label']
-        self.assertEqual(r['rdfs:label'], None)
-
-    def testGetSetDelPredicateType(self):
-        """Test getting, setting and deleting a multi-value predicate with an explicit expected RDF Class."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/offering')
-        test_subject2 = NamedNode('http://example.com/aposi1')
-        test_subject3 = NamedNode('http://example.com/aposi2')
-        test_subject4 = NamedNode('http://example.com/possip1')
-
-        shared_prefixes = {
-            'gr': 'http://purl.org/goodrelations/',
-        }
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        @pymantic.rdf.register_class('gr:ActualProductOrServiceInstance')
-        class ActualProduct(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        @pymantic.rdf.register_class('gr:ProductOrServicesSomeInstancesPlaceholder')
-        class PlaceholderProduct(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        offering = Offering.new(graph, test_subject1)
-        aposi1 = ActualProduct.new(graph, test_subject2)
-        aposi2 = ActualProduct.new(graph, test_subject3)
-        possip1 = PlaceholderProduct.new(graph, test_subject4)
-        offering['gr:includes', ActualProduct] = set((aposi1, aposi2,))
-        offering['gr:includes', PlaceholderProduct] = set((possip1,))
-        example_values = set(offering['gr:includes', ActualProduct])
-        self.assert_(aposi1 in example_values)
-        self.assert_(aposi2 in example_values)
-        self.assert_(possip1 not in example_values)
-        self.assertEqual(len(example_values), 2)
-        example_values = set(offering['gr:includes', PlaceholderProduct])
-        self.assert_(aposi1 not in example_values)
-        self.assert_(aposi2 not in example_values)
-        self.assert_(possip1 in example_values)
-        self.assertEqual(len(example_values), 1)
-        del offering['gr:includes', ActualProduct]
-        example_values = set(offering['gr:includes', ActualProduct])
-        self.assertEqual(len(example_values), 0)
-        example_values = set(offering['gr:includes', PlaceholderProduct])
-        self.assert_(aposi1 not in example_values)
-        self.assert_(aposi2 not in example_values)
-        self.assert_(possip1 in example_values)
-        self.assertEqual(len(example_values), 1)
-
-    def testGetSetDelScalarPredicateType(self):
-        """Test getting, setting, and deleting a scalar predicate with an explicit language."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/offering')
-        test_subject2 = NamedNode('http://example.com/aposi')
-        test_subject4 = NamedNode('http://example.com/possip')
-
-        shared_prefixes = {
-            'gr': 'http://purl.org/goodrelations/',
-        }
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-            scalars = frozenset(('gr:includes',))
-
-        @pymantic.rdf.register_class('gr:ActualProductOrServiceInstance')
-        class ActualProduct(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        @pymantic.rdf.register_class('gr:ProductOrServicesSomeInstancesPlaceholder')
-        class PlaceholderProduct(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        offering = Offering.new(graph, test_subject1)
-        aposi1 = ActualProduct.new(graph, test_subject2)
-        possip1 = PlaceholderProduct.new(graph, test_subject4)
-        offering['gr:includes', ActualProduct] = aposi1
-        self.assertEqual(aposi1, offering['gr:includes', ActualProduct])
-        self.assertEqual(None, offering['gr:includes', PlaceholderProduct])
-        self.assertEqual(aposi1, offering['gr:includes'])
-        offering['gr:includes', PlaceholderProduct] = possip1
-        self.assertEqual(None, offering['gr:includes', ActualProduct])
-        self.assertEqual(possip1, offering['gr:includes', PlaceholderProduct])
-        self.assertEqual(possip1, offering['gr:includes'])
-        del offering['gr:includes', ActualProduct]
-        self.assertEqual(offering['gr:includes', ActualProduct], None)
-        self.assertEqual(possip1, offering['gr:includes', PlaceholderProduct])
-        del offering['gr:includes', PlaceholderProduct]
-        self.assertEqual(offering['gr:includes', ActualProduct], None)
-        self.assertEqual(offering['gr:includes', PlaceholderProduct], None)
-        offering['gr:includes', ActualProduct] = aposi1
-        self.assertEqual(aposi1, offering['gr:includes', ActualProduct])
-        self.assertEqual(None, offering['gr:includes', PlaceholderProduct])
-        self.assertEqual(aposi1, offering['gr:includes'])
-        del offering['gr:includes']
-        self.assertEqual(None, offering['gr:includes', ActualProduct])
-        self.assertEqual(None, offering['gr:includes', PlaceholderProduct])
-        self.assertEqual(None, offering['gr:includes'])
-
-    def testSetMixedScalarPredicate(self):
-        """Test getting and setting a scalar predicate with mixed typing."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/offering')
-        test_subject2 = NamedNode('http://example.com/aposi')
-
-        shared_prefixes = {
-            'gr': 'http://purl.org/goodrelations/',
-        }
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-            scalars = frozenset(('gr:includes',))
-
-        @pymantic.rdf.register_class('gr:ActualProductOrServiceInstance')
-        class ActualProduct(pymantic.rdf.Resource):
-            prefixes = shared_prefixes
-
-        offering = Offering.new(graph, test_subject1)
-        aposi1 = ActualProduct.new(graph, test_subject2)
-        test_en = Literal('foo', language='en')
-        test_fr = Literal('le foo', language='fr')
-        test_dt = Literal('42', datatype = XSD('integer'))
-
-        offering['gr:includes'] = aposi1
-        self.assertEqual(offering['gr:includes'], aposi1)
-        offering['gr:includes'] = test_dt
-        self.assertEqual(offering['gr:includes'], test_dt)
-        self.assertEqual(offering['gr:includes', ActualProduct], None)
-        offering['gr:includes'] = test_en
-        self.assertEqual(offering['gr:includes', ActualProduct], None)
-        self.assertEqual(offering['gr:includes', XSD('integer')], None)
-        self.assertEqual(offering['gr:includes'], test_en)
-        self.assertEqual(offering['gr:includes', 'en'], test_en)
-        self.assertEqual(offering['gr:includes', 'fr'], None)
-        offering['gr:includes'] = test_fr
-        self.assertEqual(offering['gr:includes', ActualProduct], None)
-        self.assertEqual(offering['gr:includes', XSD('integer')], None)
-        self.assertEqual(offering['gr:includes'], test_en)
-        self.assertEqual(offering['gr:includes', 'en'], test_en)
-        self.assertEqual(offering['gr:includes', 'fr'], test_fr)
-        offering['gr:includes'] = aposi1
-        self.assertEqual(offering['gr:includes'], aposi1)
-        self.assertEqual(offering['gr:includes', XSD('integer')], None)
-        self.assertEqual(offering['gr:includes', 'en'], None)
-        self.assertEqual(offering['gr:includes', 'fr'], None)
-
-    def testResourcePredicate(self):
-        """Test instantiating a class when accessing a predicate."""
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        @pymantic.rdf.register_class('gr:PriceSpecification')
-        class PriceSpecification(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        test_subject1 = NamedNode('http://example.com/offering')
-        test_subject2 = NamedNode('http://example.com/price')
-        graph = Graph()
-        graph.add(Triple(test_subject1, Offering.resolve('rdf:type'),
-                         Offering.resolve('gr:Offering')))
-        graph.add(Triple(test_subject1, Offering.resolve('gr:hasPriceSpecification'),
-                         test_subject2))
-        graph.add(Triple(test_subject2, PriceSpecification.resolve('rdf:type'),
-                         PriceSpecification.resolve('gr:PriceSpecification')))
-        offering = Offering(graph, test_subject1)
-        price_specification = PriceSpecification(graph, test_subject2)
-        prices = set(offering['gr:hasPriceSpecification'])
-        self.assertEqual(len(prices), 1)
-        self.assert_(price_specification in prices)
-
-    def testResourcePredicateAssignment(self):
-        """Test assigning an instance of a resource to a predicate."""
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        @pymantic.rdf.register_class('gr:PriceSpecification')
-        class PriceSpecification(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        test_subject1 = NamedNode('http://example.com/offering')
-        test_subject2 = NamedNode('http://example.com/price')
-        graph = Graph()
-        graph.add(Triple(test_subject1, Offering.resolve('rdf:type'),
-                         Offering.resolve('gr:Offering')))
-        graph.add(Triple(test_subject2, PriceSpecification.resolve('rdf:type'),
-                         PriceSpecification.resolve('gr:PriceSpecification')))
-        offering = Offering(graph, test_subject1)
-        price_specification = PriceSpecification(graph, test_subject2)
-        before_prices = set(offering['gr:hasPriceSpecification'])
-        self.assertEqual(len(before_prices), 0)
-        offering['gr:hasPriceSpecification'] = price_specification
-        after_prices = set(offering['gr:hasPriceSpecification'])
-        self.assertEqual(len(after_prices), 1)
-        self.assert_(price_specification in after_prices)
-
-    def testNewResource(self):
-        """Test creating a new resource."""
-        graph = Graph()
-
-        @pymantic.rdf.register_class('foaf:Person')
-        class Person(pymantic.rdf.Resource):
-            prefixes = {
-                'foaf': 'http://xmlns.com/foaf/0.1/',
-            }
-
-        test_subject = NamedNode('http://example.com/')
-        p = Person.new(graph, test_subject)
-
-    def testGetAllResourcesInGraph(self):
-        """Test iterating over all of the resources in a graph with a
-        particular RDF type."""
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        graph = Graph()
-        test_subject_base = NamedNode('http://example.com/')
-        for i in range(10):
-            graph.add(Triple(NamedNode(test_subject_base + str(i)),
-                             Offering.resolve('rdf:type'),
-                             Offering.resolve('gr:Offering')))
-        offerings = Offering.in_graph(graph)
-        self.assertEqual(len(offerings), 10)
-        for i in range(10):
-            this_subject = NamedNode(test_subject_base + str(i))
-            offering = Offering(graph, this_subject)
-            self.assert_(offering in offerings)
-
-    def testContained(self):
-        """Test in against a multi-value predicate."""
-        graph = Graph()
-        test_subject1 = NamedNode('http://example.com/')
-        r = pymantic.rdf.Resource(graph, test_subject1)
-        r['rdfs:example'] = set(('foo', 'bar'))
-        self.assert_('rdfs:example' in r)
-        self.assertFalse(('rdfs:example', 'en') in r)
-        self.assertFalse(('rdfs:example', 'fr') in r)
-        self.assertFalse('rdfs:examplefoo' in r)
-        del r['rdfs:example']
-        self.assertFalse('rdfs:example' in r)
-        self.assertFalse(('rdfs:example', 'en') in r)
-        self.assertFalse(('rdfs:example', 'fr') in r)
-        self.assertFalse('rdfs:examplefoo' in r)
-        r['rdfs:example', 'fr'] = 'le foo'
-
-    def testBack(self):
-        """Test following a predicate backwards."""
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        @pymantic.rdf.register_class('gr:PriceSpecification')
-        class PriceSpecification(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        graph = Graph()
-        offering1 = Offering.new(graph, 'http://example.com/offering1')
-        offering2 = Offering.new(graph, 'http://example.com/offering2')
-        offering3 = Offering.new(graph, 'http://example.com/offering3')
-        price1 = PriceSpecification.new(graph, 'http://example.com/price1')
-        price2 = PriceSpecification.new(graph, 'http://example.com/price2')
-        price3 = PriceSpecification.new(graph, 'http://example.com/price3')
-        offering1['gr:hasPriceSpecification'] = set((price1, price2, price3,))
-        offering2['gr:hasPriceSpecification'] = set((price2, price3,))
-        self.assertEqual(set(price1.object_of(predicate='gr:hasPriceSpecification')),
-                         set((offering1,)))
-        self.assertEqual(set(price2.object_of(predicate='gr:hasPriceSpecification')),
-                         set((offering1,offering2,)))
-        self.assertEqual(set(price3.object_of(predicate='gr:hasPriceSpecification')),
-                         set((offering1,offering2,)))
-
-    def testGetAllValues(self):
-        """Test getting all values for a predicate."""
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        en = Literal('foo', language='en')
-        fr = Literal('bar', language='fr')
-        es = Literal('baz', language='es')
-        xsdstring = Literal('aap')
-        xsddecimal = Literal('9.95', datatype=XSD('decimal'))
-        graph = Graph()
-        offering = Offering.new(graph, 'http://example.com/offering')
-
-        offering['gr:description'] = set((en, fr, es,))
-        self.assertEqual(frozenset(offering['gr:description']), frozenset((en,fr,es,)))
-        self.assertEqual(frozenset(offering['gr:description', 'en']), frozenset((en,)))
-        self.assertEqual(frozenset(offering['gr:description', 'fr']), frozenset((fr,)))
-        self.assertEqual(frozenset(offering['gr:description', 'es']), frozenset((es,)))
-        self.assertEqual(frozenset(offering['gr:description', None]),
-                         frozenset((en, fr, es,)))
-
-        offering['gr:description'] = set((xsdstring, xsddecimal,))
-        self.assertEqual(frozenset(offering['gr:description', '']),
-                         frozenset((xsdstring,)))
-        self.assertEqual(frozenset(offering['gr:description', XSD('string')]),
-                         frozenset((xsdstring,)))
-        self.assertEqual(frozenset(offering['gr:description', XSD('decimal')]),
-                         frozenset((xsddecimal,)))
-        self.assertEqual(frozenset(offering['gr:description', None]),
-                         frozenset((xsdstring, xsddecimal,)))
-
-        offering['gr:description'] = set((en, fr, es, xsdstring, xsddecimal,))
-        self.assertEqual(frozenset(offering['gr:description']), frozenset((en, fr, es, xsdstring, xsddecimal,)))
-        self.assertEqual(frozenset(offering['gr:description', 'en']), frozenset((en,)))
-        self.assertEqual(frozenset(offering['gr:description', 'fr']), frozenset((fr,)))
-        self.assertEqual(frozenset(offering['gr:description', 'es']), frozenset((es,)))
-        self.assertEqual(frozenset(offering['gr:description', '']),
-                         frozenset((xsdstring,)))
-        self.assertEqual(frozenset(offering['gr:description', XSD('string')]),
-                         frozenset((xsdstring,)))
-        self.assertEqual(frozenset(offering['gr:description', XSD('decimal')]),
-                         frozenset((xsddecimal,)))
-        self.assertEqual(frozenset(offering['gr:description', None]),
-                         frozenset((en, fr, es, xsdstring, xsddecimal,)))
-
-    def testGetAllValuesScalar(self):
-        """Test getting all values for a predicate."""
-
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-            scalars = frozenset(('gr:description',))
-
-        en = Literal('foo', language='en')
-        fr = Literal('bar', language='fr')
-        es = Literal('baz', language='es')
-        graph = Graph()
-        offering = Offering.new(graph, 'http://example.com/offering')
-        offering['gr:description'] = en
-        offering['gr:description'] = fr
-        offering['gr:description'] = es
-        self.assertEqual(offering['gr:description'], en)
-        self.assertEqual(offering['gr:description', 'en'], en)
-        self.assertEqual(offering['gr:description', 'fr'], fr)
-        self.assertEqual(offering['gr:description', 'es'], es)
-        self.assertEqual(frozenset(offering['gr:description', None]),
-                         frozenset((en, fr, es,)))
-
-    def testErase(self):
-        """Test erasing an object from the graph."""
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-            scalars = frozenset(('gr:name',))
-
-        graph = Graph()
-        offering1 = Offering.new(graph, 'http://example.com/offering1')
-        offering2 = Offering.new(graph, 'http://example.com/offering2')
-        offering1['gr:name'] = 'Foo'
-        offering1['gr:description'] = set(('Baz', 'Garply',))
-        offering2['gr:name'] = 'Bar'
-        offering2['gr:description'] = set(('Aap', 'Mies',))
-        self.assert_(offering1.is_a())
-        self.assert_(offering2.is_a())
-        offering1.erase()
-        self.assertFalse(offering1.is_a())
-        self.assert_(offering2.is_a())
-        self.assertFalse(offering1['gr:name'])
-        self.assertFalse(frozenset(offering1['gr:description']))
-        self.assertEqual(offering2['gr:name'], Literal('Bar', language='en'))
-
-    def testUnboundClass(self):
-        """Test classifying objects with one or more unbound classes."""
-        @pymantic.rdf.register_class('gr:Offering')
-        class Offering(pymantic.rdf.Resource):
-            prefixes = {
-                'gr': 'http://purl.org/goodrelations/',
-            }
-
-        graph = Graph()
-        funky_class = NamedNode('http://example.com/AFunkyClass')
-        funky_subject = NamedNode('http://example.com/aFunkyResource')
-
-        offering1 = Offering.new(graph, 'http://example.com/offering1')
-        graph.add(Triple(offering1.subject, RDF('type'), funky_class))
-        self.assertEqual(type(pymantic.rdf.Resource.classify(graph, offering1.subject)),
-                         Offering)
-        graph.add(Triple(funky_subject, RDF('type'), funky_class))
-        self.assertEqual(type(pymantic.rdf.Resource.classify(graph, funky_subject)),
-                         pymantic.rdf.Resource)
+
+def testMetaResourceprefixes(reset_metaresource):
+    """Test the handling of prefixes by MetaResource."""
+
+    class Foo(metaclass=pymantic.rdf.MetaResource):
+        prefixes = {
+            "foo": "bar",
+            "baz": "garply",
+            "meme": "lolcatz!",
+        }
+
+    assert Foo.prefixes == {
+        "foo": Prefix("bar"),
+        "baz": Prefix("garply"),
+        "meme": Prefix("lolcatz!"),
+    }
+
+
+def testMetaResourcePrefixInheritance(reset_metaresource):
+    """Test the composition of Prefix dictionaries by MetaResource."""
+
+    class Foo(metaclass=pymantic.rdf.MetaResource):
+        prefixes = {
+            "foo": "bar",
+            "baz": "garply",
+            "meme": "lolcatz!",
+        }
+
+    class Bar(Foo):
+        prefixes = {
+            "allyourbase": "arebelongtous!",
+            "bunny": "pancake",
+        }
+
+    assert Foo.prefixes == {
+        "foo": Prefix("bar"),
+        "baz": Prefix("garply"),
+        "meme": Prefix("lolcatz!"),
+    }
+    assert Bar.prefixes == {
+        "foo": Prefix("bar"),
+        "baz": Prefix("garply"),
+        "meme": Prefix("lolcatz!"),
+        "allyourbase": Prefix("arebelongtous!"),
+        "bunny": Prefix("pancake"),
+    }
+
+
+def testMetaResourcePrefixInheritanceReplacement(reset_metaresource):
+    """Test the composition of Prefix dictionaries by MetaResource where
+    some prefixes on the parent get replaced."""
+
+    class Foo(metaclass=pymantic.rdf.MetaResource):
+        prefixes = {
+            "foo": "bar",
+            "baz": "garply",
+            "meme": "lolcatz!",
+        }
+
+    class Bar(Foo):
+        prefixes = {
+            "allyourbase": "arebelongtous!",
+            "bunny": "pancake",
+            "foo": "notbar",
+            "baz": "notgarply",
+        }
+
+    assert Foo.prefixes == {
+        "foo": Prefix("bar"),
+        "baz": Prefix("garply"),
+        "meme": Prefix("lolcatz!"),
+    }
+    assert Bar.prefixes == {
+        "foo": Prefix("notbar"),
+        "baz": Prefix("notgarply"),
+        "meme": Prefix("lolcatz!"),
+        "allyourbase": Prefix("arebelongtous!"),
+        "bunny": Prefix("pancake"),
+    }
+
+
+def testResourceEquality(reset_metaresource):
+    graph = Graph()
+    otherGraph = Graph()
+    testResource = pymantic.rdf.Resource(graph, "foo")
+    assert testResource == pymantic.rdf.Resource(graph, "foo")
+    assert testResource == NamedNode("foo")
+    assert testResource == "foo"
+    assert testResource != pymantic.rdf.Resource(graph, "bar")
+    assert testResource == pymantic.rdf.Resource(otherGraph, "foo")
+    assert testResource != NamedNode("bar")
+    assert testResource != "bar"
+    assert testResource != 42
+
+
+def testClassification(reset_metaresource):
+    """Test classification of a resource."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    test_subject = NamedNode("http://example.com/athing")
+    graph = Graph()
+    graph.add(
+        Triple(
+            test_subject,
+            Offering.resolve("rdf:type"),
+            Offering.resolve("gr:Offering"),
+        )
+    )
+    offering = pymantic.rdf.Resource.classify(graph, test_subject)
+    assert isinstance(offering, Offering)
+
+
+def testMulticlassClassification(reset_metaresource):
+    """Test classification of a resource that matches multiple registered
+    classes."""
+
+    @pymantic.rdf.register_class("foaf:Organization")
+    class Organization(pymantic.rdf.Resource):
+        prefixes = {
+            "foaf": "http://xmlns.com/foaf/0.1/",
+        }
+
+    @pymantic.rdf.register_class("foaf:Group")
+    class Group(pymantic.rdf.Resource):
+        prefixes = {
+            "foaf": "http://xmlns.com/foaf/0.1/",
+        }
+
+    test_subject1 = NamedNode("http://example.com/aorganization")
+    test_subject2 = NamedNode("http://example.com/agroup")
+    test_subject3 = NamedNode("http://example.com/aorgandgroup")
+    graph = Graph()
+    graph.add(
+        Triple(
+            test_subject1,
+            Organization.resolve("rdf:type"),
+            Organization.resolve("foaf:Organization"),
+        )
+    )
+    graph.add(
+        Triple(test_subject2, Group.resolve("rdf:type"), Group.resolve("foaf:Group"))
+    )
+    graph.add(
+        Triple(
+            test_subject3,
+            Organization.resolve("rdf:type"),
+            Organization.resolve("foaf:Organization"),
+        )
+    )
+    graph.add(
+        Triple(
+            test_subject3,
+            Organization.resolve("rdf:type"),
+            Organization.resolve("foaf:Group"),
+        )
+    )
+    organization = pymantic.rdf.Resource.classify(graph, test_subject1)
+    group = pymantic.rdf.Resource.classify(graph, test_subject2)
+    both = pymantic.rdf.Resource.classify(graph, test_subject3)
+    assert isinstance(organization, Organization)
+    assert not isinstance(group, Organization)
+    assert not isinstance(organization, Group)
+    assert isinstance(group, Group)
+    assert isinstance(both, Organization)
+    assert isinstance(both, Group)
+
+
+def testStr(reset_metaresource):
+    """Test str-y serialization of Resources."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/aorganization")
+    test_label = Literal("Test Label", language="en")
+    graph.add(
+        Triple(test_subject1, pymantic.rdf.Resource.resolve("rdfs:label"), test_label)
+    )
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    assert r["rdfs:label"] == test_label
+    assert str(r) == test_label.value
+
+
+def testGetSetDelPredicate(reset_metaresource):
+    """Test getting, setting, and deleting a multi-value predicate."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    r["rdfs:example"] = set(("foo", "bar"))
+    example_values = set(r["rdfs:example"])
+    assert Literal("foo") in example_values
+    assert Literal("bar") in example_values
+    assert len(example_values) == 2
+    del r["rdfs:example"]
+    example_values = set(r["rdfs:example"])
+    assert len(example_values) == 0
+
+
+def testGetSetDelScalarPredicate(reset_metaresource):
+    """Test getting, setting, and deleting a scalar predicate."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    r["rdfs:label"] = "foo"
+    assert r["rdfs:label"] == Literal("foo", language="en")
+    del r["rdfs:label"]
+    assert r["rdfs:label"] is None
+
+
+def testGetSetDelPredicateLanguage(reset_metaresource):
+    """Test getting, setting and deleting a multi-value predicate with an explicit language."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    r["rdfs:example", "en"] = set(("baz",))
+    r["rdfs:example", "fr"] = set(("foo", "bar"))
+    example_values = set(r["rdfs:example", "fr"])
+    assert Literal("foo", language="fr") in example_values
+    assert Literal("bar", language="fr") in example_values
+    assert Literal("baz", language="en") not in example_values
+    assert len(example_values) == 2
+    example_values = set(r["rdfs:example", "en"])
+    assert Literal("foo", language="fr") not in example_values
+    assert Literal("bar", language="fr") not in example_values
+    assert Literal("baz", language="en") in example_values
+    assert len(example_values) == 1
+    del r["rdfs:example", "fr"]
+    example_values = set(r["rdfs:example", "fr"])
+    assert len(example_values) == 0
+    example_values = set(r["rdfs:example", "en"])
+    assert Literal("foo", language="fr") not in example_values
+    assert Literal("bar", language="fr") not in example_values
+    assert Literal("baz", language="en") in example_values
+    assert len(example_values) == 1
+
+
+def testGetSetDelScalarPredicateLanguage(reset_metaresource):
+    """Test getting, setting, and deleting a scalar predicate with an explicit language."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    r["rdfs:label"] = "foo"
+    r["rdfs:label", "fr"] = "bar"
+    assert r["rdfs:label"] == Literal("foo", language="en")
+    assert r["rdfs:label", "en"] == Literal("foo", language="en")
+    assert r["rdfs:label", "fr"] == Literal("bar", language="fr")
+    del r["rdfs:label"]
+    assert r["rdfs:label"] is None
+    assert r["rdfs:label", "en"] is None
+    assert r["rdfs:label", "fr"] == Literal("bar", language="fr")
+
+
+def testGetSetDelPredicateDatatype(reset_metaresource):
+    """Test getting, setting and deleting a multi-value predicate with an explicit datatype."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    now = datetime.datetime.now()
+    then = datetime.datetime.now() - datetime.timedelta(days=1)
+    number = 42
+    r["rdfs:example", XSD("integer")] = set((number,))
+    r["rdfs:example", XSD("dateTime")] = set(
+        (
+            now,
+            then,
+        )
+    )
+    example_values = set(r["rdfs:example", XSD("dateTime")])
+    assert Literal(now) in example_values
+    assert Literal(then) in example_values
+    assert Literal(number) not in example_values
+    assert len(example_values) == 2
+    example_values = set(r["rdfs:example", XSD("integer")])
+    assert Literal(now) not in example_values
+    assert Literal(then) not in example_values
+    assert Literal(number) in example_values
+    assert len(example_values) == 1
+    del r["rdfs:example", XSD("dateTime")]
+    example_values = set(r["rdfs:example", XSD("dateTime")])
+    assert len(example_values) == 0
+    example_values = set(r["rdfs:example", XSD("integer")])
+    assert Literal(now) not in example_values
+    assert Literal(then) not in example_values
+    assert Literal(number) in example_values
+    assert len(example_values) == 1
+
+
+def testGetSetDelScalarPredicateDatatype(reset_metaresource):
+    """Test getting, setting, and deleting a scalar predicate with an explicit datatype."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    now = datetime.datetime.now()
+    number = 42
+    r["rdfs:label", XSD("integer")] = number
+    assert r["rdfs:label", XSD("integer")] == Literal(number, datatype=XSD("integer"))
+    assert r["rdfs:label", XSD("dateTime")] is None
+    assert r["rdfs:label"] == Literal(number, datatype=XSD("integer"))
+    r["rdfs:label", XSD("dateTime")] = now
+    assert r["rdfs:label", XSD("dateTime")] == Literal(now)
+    assert r["rdfs:label", XSD("integer")] is None
+    assert r["rdfs:label"] == Literal(now)
+    del r["rdfs:label", XSD("integer")]
+    assert r["rdfs:label", XSD("dateTime")] == Literal(now)
+    assert r["rdfs:label", XSD("integer")] is None
+    assert r["rdfs:label"] == Literal(now)
+    del r["rdfs:label", XSD("dateTime")]
+    assert r["rdfs:label"] is None
+    r["rdfs:label", XSD("integer")] = number
+    assert r["rdfs:label", XSD("integer")] == Literal(number, datatype=XSD("integer"))
+    assert r["rdfs:label", XSD("dateTime")] is None
+    assert r["rdfs:label"] == Literal(number, datatype=XSD("integer"))
+    del r["rdfs:label"]
+    assert r["rdfs:label"] is None
+
+
+def testGetSetDelPredicateType(reset_metaresource):
+    """Test getting, setting and deleting a multi-value predicate with an explicit expected RDF Class."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/offering")
+    test_subject2 = NamedNode("http://example.com/aposi1")
+    test_subject3 = NamedNode("http://example.com/aposi2")
+    test_subject4 = NamedNode("http://example.com/possip1")
+
+    shared_prefixes = {
+        "gr": "http://purl.org/goodrelations/",
+    }
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    @pymantic.rdf.register_class("gr:ActualProductOrServiceInstance")
+    class ActualProduct(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    @pymantic.rdf.register_class("gr:ProductOrServicesSomeInstancesPlaceholder")
+    class PlaceholderProduct(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    offering = Offering.new(graph, test_subject1)
+    aposi1 = ActualProduct.new(graph, test_subject2)
+    aposi2 = ActualProduct.new(graph, test_subject3)
+    possip1 = PlaceholderProduct.new(graph, test_subject4)
+    offering["gr:includes", ActualProduct] = set(
+        (
+            aposi1,
+            aposi2,
+        )
+    )
+    offering["gr:includes", PlaceholderProduct] = set((possip1,))
+    example_values = set(offering["gr:includes", ActualProduct])
+    assert aposi1 in example_values
+    assert aposi2 in example_values
+    assert possip1 not in example_values
+    assert len(example_values) == 2
+    example_values = set(offering["gr:includes", PlaceholderProduct])
+    assert aposi1 not in example_values
+    assert aposi2 not in example_values
+    assert possip1 in example_values
+    assert len(example_values) == 1
+    del offering["gr:includes", ActualProduct]
+    example_values = set(offering["gr:includes", ActualProduct])
+    assert len(example_values) == 0
+    example_values = set(offering["gr:includes", PlaceholderProduct])
+    assert aposi1 not in example_values
+    assert aposi2 not in example_values
+    assert possip1 in example_values
+    assert len(example_values) == 1
+
+
+def testGetSetDelScalarPredicateType(reset_metaresource):
+    """Test getting, setting, and deleting a scalar predicate with an explicit language."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/offering")
+    test_subject2 = NamedNode("http://example.com/aposi")
+    test_subject4 = NamedNode("http://example.com/possip")
+
+    shared_prefixes = {
+        "gr": "http://purl.org/goodrelations/",
+    }
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+        scalars = frozenset(("gr:includes",))
+
+    @pymantic.rdf.register_class("gr:ActualProductOrServiceInstance")
+    class ActualProduct(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    @pymantic.rdf.register_class("gr:ProductOrServicesSomeInstancesPlaceholder")
+    class PlaceholderProduct(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    offering = Offering.new(graph, test_subject1)
+    aposi1 = ActualProduct.new(graph, test_subject2)
+    possip1 = PlaceholderProduct.new(graph, test_subject4)
+    offering["gr:includes", ActualProduct] = aposi1
+    assert aposi1 == offering["gr:includes", ActualProduct]
+    assert offering["gr:includes", PlaceholderProduct] is None
+    assert aposi1 == offering["gr:includes"]
+    offering["gr:includes", PlaceholderProduct] = possip1
+    assert offering["gr:includes", ActualProduct] is None
+    assert possip1 == offering["gr:includes", PlaceholderProduct]
+    assert possip1 == offering["gr:includes"]
+    del offering["gr:includes", ActualProduct]
+    assert offering["gr:includes", ActualProduct] is None
+    assert possip1 == offering["gr:includes", PlaceholderProduct]
+    del offering["gr:includes", PlaceholderProduct]
+    assert offering["gr:includes", ActualProduct] is None
+    assert offering["gr:includes", PlaceholderProduct] is None
+    offering["gr:includes", ActualProduct] = aposi1
+    assert aposi1 == offering["gr:includes", ActualProduct]
+    assert offering["gr:includes", PlaceholderProduct] is None
+    assert aposi1 == offering["gr:includes"]
+    del offering["gr:includes"]
+    assert offering["gr:includes", ActualProduct] is None
+    assert offering["gr:includes", PlaceholderProduct] is None
+    assert offering["gr:includes"] is None
+
+
+def testSetMixedScalarPredicate(reset_metaresource):
+    """Test getting and setting a scalar predicate with mixed typing."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/offering")
+    test_subject2 = NamedNode("http://example.com/aposi")
+
+    shared_prefixes = {
+        "gr": "http://purl.org/goodrelations/",
+    }
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+        scalars = frozenset(("gr:includes",))
+
+    @pymantic.rdf.register_class("gr:ActualProductOrServiceInstance")
+    class ActualProduct(pymantic.rdf.Resource):
+        prefixes = shared_prefixes
+
+    offering = Offering.new(graph, test_subject1)
+    aposi1 = ActualProduct.new(graph, test_subject2)
+    test_en = Literal("foo", language="en")
+    test_fr = Literal("le foo", language="fr")
+    test_dt = Literal("42", datatype=XSD("integer"))
+
+    offering["gr:includes"] = aposi1
+    assert offering["gr:includes"] == aposi1
+    offering["gr:includes"] = test_dt
+    assert offering["gr:includes"] == test_dt
+    assert offering["gr:includes", ActualProduct] is None
+    offering["gr:includes"] = test_en
+    assert offering["gr:includes", ActualProduct] is None
+    assert offering["gr:includes", XSD("integer")] is None
+    assert offering["gr:includes"] == test_en
+    assert offering["gr:includes", "en"] == test_en
+    assert offering["gr:includes", "fr"] is None
+    offering["gr:includes"] = test_fr
+    assert offering["gr:includes", ActualProduct] is None
+    assert offering["gr:includes", XSD("integer")] is None
+    assert offering["gr:includes"] == test_en
+    assert offering["gr:includes", "en"] == test_en
+    assert offering["gr:includes", "fr"] == test_fr
+    offering["gr:includes"] = aposi1
+    assert offering["gr:includes"] == aposi1
+    assert offering["gr:includes", XSD("integer")] is None
+    assert offering["gr:includes", "en"] is None
+    assert offering["gr:includes", "fr"] is None
+
+
+def testResourcePredicate(reset_metaresource):
+    """Test instantiating a class when accessing a predicate."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    @pymantic.rdf.register_class("gr:PriceSpecification")
+    class PriceSpecification(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    test_subject1 = NamedNode("http://example.com/offering")
+    test_subject2 = NamedNode("http://example.com/price")
+    graph = Graph()
+    graph.add(
+        Triple(
+            test_subject1,
+            Offering.resolve("rdf:type"),
+            Offering.resolve("gr:Offering"),
+        )
+    )
+    graph.add(
+        Triple(
+            test_subject1,
+            Offering.resolve("gr:hasPriceSpecification"),
+            test_subject2,
+        )
+    )
+    graph.add(
+        Triple(
+            test_subject2,
+            PriceSpecification.resolve("rdf:type"),
+            PriceSpecification.resolve("gr:PriceSpecification"),
+        )
+    )
+    offering = Offering(graph, test_subject1)
+    price_specification = PriceSpecification(graph, test_subject2)
+    prices = set(offering["gr:hasPriceSpecification"])
+    assert len(prices) == 1
+    assert price_specification in prices
+
+
+def testResourcePredicateAssignment(reset_metaresource):
+    """Test assigning an instance of a resource to a predicate."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    @pymantic.rdf.register_class("gr:PriceSpecification")
+    class PriceSpecification(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    test_subject1 = NamedNode("http://example.com/offering")
+    test_subject2 = NamedNode("http://example.com/price")
+    graph = Graph()
+    graph.add(
+        Triple(
+            test_subject1,
+            Offering.resolve("rdf:type"),
+            Offering.resolve("gr:Offering"),
+        )
+    )
+    graph.add(
+        Triple(
+            test_subject2,
+            PriceSpecification.resolve("rdf:type"),
+            PriceSpecification.resolve("gr:PriceSpecification"),
+        )
+    )
+    offering = Offering(graph, test_subject1)
+    price_specification = PriceSpecification(graph, test_subject2)
+    before_prices = set(offering["gr:hasPriceSpecification"])
+    assert len(before_prices) == 0
+    offering["gr:hasPriceSpecification"] = price_specification
+    after_prices = set(offering["gr:hasPriceSpecification"])
+    assert len(after_prices) == 1
+    assert price_specification in after_prices
+
+
+def testNewResource(reset_metaresource):
+    """Test creating a new resource."""
+    graph = Graph()
+
+    @pymantic.rdf.register_class("foaf:Person")
+    class Person(pymantic.rdf.Resource):
+        prefixes = {
+            "foaf": "http://xmlns.com/foaf/0.1/",
+        }
+
+    test_subject = NamedNode("http://example.com/")
+    Person.new(graph, test_subject)
+
+
+def testGetAllResourcesInGraph(reset_metaresource):
+    """Test iterating over all of the resources in a graph with a
+    particular RDF type."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    graph = Graph()
+    test_subject_base = NamedNode("http://example.com/")
+    for i in range(10):
+        graph.add(
+            Triple(
+                NamedNode(test_subject_base + str(i)),
+                Offering.resolve("rdf:type"),
+                Offering.resolve("gr:Offering"),
+            )
+        )
+    offerings = Offering.in_graph(graph)
+    assert len(offerings) == 10
+    for i in range(10):
+        this_subject = NamedNode(test_subject_base + str(i))
+        offering = Offering(graph, this_subject)
+        assert offering in offerings
+
+
+def testContained(reset_metaresource):
+    """Test in against a multi-value predicate."""
+    graph = Graph()
+    test_subject1 = NamedNode("http://example.com/")
+    r = pymantic.rdf.Resource(graph, test_subject1)
+    r["rdfs:example"] = set(("foo", "bar"))
+    assert "rdfs:example" in r
+    assert ("rdfs:example", "en") not in r
+    ("rdfs:example", "fr") not in r
+    assert "rdfs:examplefoo" not in r
+    del r["rdfs:example"]
+    assert "rdfs:example" not in r
+    assert ("rdfs:example", "en") not in r
+    assert ("rdfs:example", "fr") not in r
+    assert "rdfs:examplefoo" not in r
+    r["rdfs:example", "fr"] = "le foo"
+
+
+def testBack(reset_metaresource):
+    """Test following a predicate backwards."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    @pymantic.rdf.register_class("gr:PriceSpecification")
+    class PriceSpecification(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    graph = Graph()
+    offering1 = Offering.new(graph, "http://example.com/offering1")
+    offering2 = Offering.new(graph, "http://example.com/offering2")
+    Offering.new(graph, "http://example.com/offering3")
+    price1 = PriceSpecification.new(graph, "http://example.com/price1")
+    price2 = PriceSpecification.new(graph, "http://example.com/price2")
+    price3 = PriceSpecification.new(graph, "http://example.com/price3")
+    offering1["gr:hasPriceSpecification"] = set(
+        (
+            price1,
+            price2,
+            price3,
+        )
+    )
+    offering2["gr:hasPriceSpecification"] = set(
+        (
+            price2,
+            price3,
+        )
+    )
+    assert set(price1.object_of(predicate="gr:hasPriceSpecification")) == set(
+        (offering1,)
+    )
+    assert set(price2.object_of(predicate="gr:hasPriceSpecification")) == set(
+        (
+            offering1,
+            offering2,
+        )
+    )
+    assert set(price3.object_of(predicate="gr:hasPriceSpecification")) == set(
+        (
+            offering1,
+            offering2,
+        )
+    )
+
+
+def testGetAllValues(reset_metaresource):
+    """Test getting all values for a predicate."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    en = Literal("foo", language="en")
+    fr = Literal("bar", language="fr")
+    es = Literal("baz", language="es")
+    xsdstring = Literal("aap")
+    xsddecimal = Literal("9.95", datatype=XSD("decimal"))
+    graph = Graph()
+    offering = Offering.new(graph, "http://example.com/offering")
+
+    offering["gr:description"] = set(
+        (
+            en,
+            fr,
+            es,
+        )
+    )
+    assert frozenset(offering["gr:description"]) == frozenset(
+        (
+            en,
+            fr,
+            es,
+        )
+    )
+    assert frozenset(offering["gr:description", "en"]) == frozenset((en,))
+    assert frozenset(offering["gr:description", "fr"]) == frozenset((fr,))
+    assert frozenset(offering["gr:description", "es"]) == frozenset((es,))
+    assert frozenset(offering["gr:description", None]) == frozenset(
+        (
+            en,
+            fr,
+            es,
+        )
+    )
+
+    offering["gr:description"] = set(
+        (
+            xsdstring,
+            xsddecimal,
+        )
+    )
+    assert frozenset(offering["gr:description", ""]), frozenset((xsdstring,))
+    assert frozenset(offering["gr:description", XSD("string")]) == frozenset(
+        (xsdstring,)
+    )
+    assert frozenset(offering["gr:description", XSD("decimal")]) == frozenset(
+        (xsddecimal,)
+    )
+    assert frozenset(offering["gr:description", None]) == frozenset(
+        (
+            xsdstring,
+            xsddecimal,
+        )
+    )
+
+    offering["gr:description"] = set(
+        (
+            en,
+            fr,
+            es,
+            xsdstring,
+            xsddecimal,
+        )
+    )
+    assert frozenset(offering["gr:description"]) == frozenset(
+        (
+            en,
+            fr,
+            es,
+            xsdstring,
+            xsddecimal,
+        )
+    )
+    assert frozenset(offering["gr:description", "en"]) == frozenset((en,))
+    assert frozenset(offering["gr:description", "fr"]) == frozenset((fr,))
+    assert frozenset(offering["gr:description", "es"]) == frozenset((es,))
+    assert frozenset(offering["gr:description", ""]) == frozenset((xsdstring,))
+    assert frozenset(offering["gr:description", XSD("string")]) == frozenset(
+        (xsdstring,)
+    )
+    assert frozenset(offering["gr:description", XSD("decimal")]) == frozenset(
+        (xsddecimal,)
+    )
+    assert frozenset(offering["gr:description", None]) == frozenset(
+        (
+            en,
+            fr,
+            es,
+            xsdstring,
+            xsddecimal,
+        )
+    )
+
+
+def testGetAllValuesScalar(reset_metaresource):
+    """Test getting all values for a predicate."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+        scalars = frozenset(("gr:description",))
+
+    en = Literal("foo", language="en")
+    fr = Literal("bar", language="fr")
+    es = Literal("baz", language="es")
+    graph = Graph()
+    offering = Offering.new(graph, "http://example.com/offering")
+    offering["gr:description"] = en
+    offering["gr:description"] = fr
+    offering["gr:description"] = es
+    assert offering["gr:description"] == en
+    assert offering["gr:description", "en"] == en
+    assert offering["gr:description", "fr"] == fr
+    assert offering["gr:description", "es"] == es
+    assert frozenset(offering["gr:description", None]) == frozenset(
+        (
+            en,
+            fr,
+            es,
+        )
+    )
+
+
+def testErase(reset_metaresource):
+    """Test erasing an object from the graph."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+        scalars = frozenset(("gr:name",))
+
+    graph = Graph()
+    offering1 = Offering.new(graph, "http://example.com/offering1")
+    offering2 = Offering.new(graph, "http://example.com/offering2")
+    offering1["gr:name"] = "Foo"
+    offering1["gr:description"] = set(
+        (
+            "Baz",
+            "Garply",
+        )
+    )
+    offering2["gr:name"] = "Bar"
+    offering2["gr:description"] = set(
+        (
+            "Aap",
+            "Mies",
+        )
+    )
+    assert offering1.is_a()
+    assert offering2.is_a()
+    offering1.erase()
+    assert not offering1.is_a()
+    assert offering2.is_a()
+    assert not offering1["gr:name"]
+    assert not frozenset(offering1["gr:description"])
+    assert offering2["gr:name"] == Literal("Bar", language="en")
+
+
+def testUnboundClass(reset_metaresource):
+    """Test classifying objects with one or more unbound classes."""
+
+    @pymantic.rdf.register_class("gr:Offering")
+    class Offering(pymantic.rdf.Resource):
+        prefixes = {
+            "gr": "http://purl.org/goodrelations/",
+        }
+
+    graph = Graph()
+    funky_class = NamedNode("http://example.com/AFunkyClass")
+    funky_subject = NamedNode("http://example.com/aFunkyResource")
+
+    offering1 = Offering.new(graph, "http://example.com/offering1")
+    graph.add(Triple(offering1.subject, RDF("type"), funky_class))
+    assert isinstance(
+        pymantic.rdf.Resource.classify(graph, offering1.subject), Offering
+    )
+    graph.add(Triple(funky_subject, RDF("type"), funky_class))
+    assert isinstance(
+        pymantic.rdf.Resource.classify(graph, funky_subject),
+        pymantic.rdf.Resource,
+    )
```

### Comparing `pymantic-0.3.0/pymantic/tests/test_parsers.py` & `pymantic-1.0.0/tests/test_parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,190 @@
-from pymantic.compat.moves import cStringIO as StringIO
-from nose.tools import *
-from nose.plugins.skip import Skip, SkipTest
-from pymantic.parsers import *
-from pymantic.primitives import *
+from io import StringIO
+
+from pymantic.parsers import (
+    jsonld_parser,
+    nquads_parser,
+    ntriples_parser,
+    turtle_parser,
+)
+from pymantic.primitives import Graph, Literal, NamedNode, Quad, Triple
+
 
 def test_parse_ntriples_named_nodes():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> <http://example.com/objects/2> .
 <http://example.com/objects/2> <http://example.com/predicates/2> <http://example.com/objects/1> .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    assert Triple(NamedNode('http://example.com/objects/1'),
-                  NamedNode('http://example.com/predicates/1'),
-                  NamedNode('http://example.com/objects/2')) in g
-    assert Triple(NamedNode('http://example.com/objects/2'),
-                  NamedNode('http://example.com/predicates/2'),
-                  NamedNode('http://example.com/objects/1')) in g
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            NamedNode("http://example.com/objects/2"),
+        )
+        in g
+    )
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            NamedNode("http://example.com/objects/1"),
+        )
+        in g
+    )
+
 
 def test_parse_ntriples_bare_literals():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> "Foo" .
 <http://example.com/objects/2> <http://example.com/predicates/2> "Bar" .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    assert Triple(NamedNode('http://example.com/objects/1'),
-                  NamedNode('http://example.com/predicates/1'),
-                  Literal("Foo")) in g
-    assert Triple(NamedNode('http://example.com/objects/2'),
-                  NamedNode('http://example.com/predicates/2'),
-                  Literal("Bar")) in g
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            Literal("Foo"),
+        )
+        in g
+    )
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            Literal("Bar"),
+        )
+        in g
+    )
+
 
 def test_parse_ntriples_language_literals():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> "Foo"@en-US .
 <http://example.com/objects/2> <http://example.com/predicates/2> "Bar"@fr .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    assert Triple(NamedNode('http://example.com/objects/1'),
-                  NamedNode('http://example.com/predicates/1'),
-                  Literal("Foo", language='en-US')) in g
-    assert Triple(NamedNode('http://example.com/objects/2'),
-                  NamedNode('http://example.com/predicates/2'),
-                  Literal("Bar", language='fr')) in g
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            Literal("Foo", language="en-US"),
+        )
+        in g
+    )
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            Literal("Bar", language="fr"),
+        )
+        in g
+    )
+
 
 def test_parse_ntriples_datatyped_literals():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> "Foo"^^<http://www.w3.org/2001/XMLSchema#string> .
 <http://example.com/objects/2> <http://example.com/predicates/2> "9.99"^^<http://www.w3.org/2001/XMLSchema#decimal> .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    assert Triple(NamedNode('http://example.com/objects/1'),
-                  NamedNode('http://example.com/predicates/1'),
-                  Literal("Foo", datatype=NamedNode('http://www.w3.org/2001/XMLSchema#string'))) in g
-    assert Triple(NamedNode('http://example.com/objects/2'),
-                  NamedNode('http://example.com/predicates/2'),
-                  Literal("9.99", datatype=NamedNode('http://www.w3.org/2001/XMLSchema#decimal'))) in g
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            Literal(
+                "Foo", datatype=NamedNode("http://www.w3.org/2001/XMLSchema#string")
+            ),
+        )
+        in g
+    )
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            Literal(
+                "9.99", datatype=NamedNode("http://www.w3.org/2001/XMLSchema#decimal")
+            ),
+        )
+        in g
+    )
+
 
 def test_parse_ntriples_mixed_literals():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> "Foo"@en-US .
 <http://example.com/objects/2> <http://example.com/predicates/2> "9.99"^^<http://www.w3.org/2001/XMLSchema#decimal> .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    assert Triple(NamedNode('http://example.com/objects/1'),
-                  NamedNode('http://example.com/predicates/1'),
-                  Literal("Foo", language='en-US')) in g
-    assert Triple(NamedNode('http://example.com/objects/2'),
-                  NamedNode('http://example.com/predicates/2'),
-                  Literal("9.99", datatype=NamedNode('http://www.w3.org/2001/XMLSchema#decimal'))) in g
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            Literal("Foo", language="en-US"),
+        )
+        in g
+    )
+    assert (
+        Triple(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            Literal(
+                "9.99", datatype=NamedNode("http://www.w3.org/2001/XMLSchema#decimal")
+            ),
+        )
+        in g
+    )
+
 
 def test_parse_ntriples_bnodes():
     test_ntriples = """<http://example.com/objects/1> <http://example.com/predicates/1> _:A1 .
 _:A1 <http://example.com/predicates/2> <http://example.com/objects/1> .
 """
     g = Graph()
     ntriples_parser.parse(StringIO(test_ntriples), g)
     assert len(g) == 2
-    #assert Triple(NamedNode('http://example.com/objects/1'),
-                  #NamedNode('http://example.com/predicates/1'),
-                  #NamedNode('http://example.com/objects/2')) in g
-    #assert Triple(NamedNode('http://example.com/objects/2'),
-                  #NamedNode('http://example.com/predicates/2'),
-                  #NamedNode('http://example.com/objects/1')) in g
+    # assert Triple(NamedNode('http://example.com/objects/1'),
+    # NamedNode('http://example.com/predicates/1'),
+    # NamedNode('http://example.com/objects/2')) in g
+    # assert Triple(NamedNode('http://example.com/objects/2'),
+    # NamedNode('http://example.com/predicates/2'),
+    # NamedNode('http://example.com/objects/1')) in g
+
 
 def test_parse_nquads_named_nodes():
     test_nquads = """<http://example.com/objects/1> <http://example.com/predicates/1> <http://example.com/objects/2> <http://example.com/graphs/1> .
 <http://example.com/objects/2> <http://example.com/predicates/2> <http://example.com/objects/1> <http://example.com/graphs/1> .
 """
     g = Graph()
     nquads_parser.parse(StringIO(test_nquads), g)
     assert len(g) == 2
-    assert Quad(NamedNode('http://example.com/objects/1'),
-                NamedNode('http://example.com/predicates/1'),
-                NamedNode('http://example.com/objects/2'),
-                NamedNode('http://example.com/graphs/1')) in g
-    assert Quad(NamedNode('http://example.com/objects/2'),
-                NamedNode('http://example.com/predicates/2'),
-                NamedNode('http://example.com/objects/1'),
-                NamedNode('http://example.com/graphs/1')) in g
+    assert (
+        Quad(
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/predicates/1"),
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/graphs/1"),
+        )
+        in g
+    )
+    assert (
+        Quad(
+            NamedNode("http://example.com/objects/2"),
+            NamedNode("http://example.com/predicates/2"),
+            NamedNode("http://example.com/objects/1"),
+            NamedNode("http://example.com/graphs/1"),
+        )
+        in g
+    )
+
 
 def test_parse_turtle_example_1():
     ttl = """@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix dc: <http://purl.org/dc/elements/1.1/> .
 @prefix ex: <http://example.org/stuff/1.0/> .
 
 <http://www.w3.org/TR/rdf-syntax-grammar>
@@ -118,14 +196,15 @@
     g = Graph()
     turtle_parser.parse(ttl, g)
     assert len(g) == 4
 
 
 def test_jsonld_basic():
     import json
+
     jsonld = """[{
   "@id": "http://example.com/id1",
   "@type": ["http://example.com/t1"],
   "http://example.com/term1": ["v1"],
   "http://example.com/term2": [{"@value": "v2", "@type": "http://example.com/t2"}],
   "http://example.com/term3": [{"@value": "v3", "@language": "en"}],
   "http://example.com/term4": [4],
```

### Comparing `pymantic-0.3.0/pymantic/tests/test_primitives.py` & `pymantic-1.0.0/tests/test_primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,288 @@
-from nose.tools import *
-from pymantic.primitives import *
 import random
 
+from pymantic.primitives import (
+    BlankNode,
+    Dataset,
+    Graph,
+    Literal,
+    NamedNode,
+    Quad,
+    Triple,
+    to_curie,
+)
+
+
 def en(s):
     return Literal(s, "en")
 
+
 def test_to_curie_multi_match():
     """Test that the longest match for prefix is used"""
-    namespaces = {'short': "aa", 'long': "aaa"}
+    namespaces = {"short": "aa", "long": "aaa"}
     curie = to_curie("aaab", namespaces)
-    assert curie == 'long:b'
+    assert curie == "long:b"
+
 
 def test_simple_add():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     assert t in g
 
+
 def test_simple_remove():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     g.remove(t)
     assert t not in g
 
+
 def test_match_VVV_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(None, None, None)
     assert t in matches
 
+
 def test_match_sVV_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(NamedNode("http://example.com"), None, None)
     assert t in matches
 
+
 def test_match_sVo_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(NamedNode("http://example.com"), None, en("Never!"))
     assert t in matches
 
+
 def test_match_spV_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
-    matches = g.match(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"), None)
+    matches = g.match(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        None,
+    )
     assert t in matches
 
+
 def test_match_Vpo_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(None, NamedNode("http://purl.org/dc/terms/issued"), en("Never!"))
     assert t in matches
 
+
 def test_match_VVo_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(None, None, en("Never!"))
     assert t in matches
 
+
 def test_match_VpV_pattern():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),en("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        en("Never!"),
+    )
     g = Graph()
     g.add(t)
     matches = g.match(None, NamedNode("http://purl.org/dc/terms/issued"), None)
     assert t in matches
 
+
 def generate_triples(n=10):
-    for i in range(1,n):
-        yield Triple(NamedNode("http://example/" + str(random.randint(1,1000))),
-                   NamedNode("http://example/terms/" + str(random.randint(1,1000))),
-                   Literal(random.randint(1,1000)))
+    for i in range(1, n):
+        yield Triple(
+            NamedNode("http://example/" + str(random.randint(1, 1000))),
+            NamedNode("http://example/terms/" + str(random.randint(1, 1000))),
+            Literal(random.randint(1, 1000)),
+        )
+
 
 def test_10000_triples():
     n = 10000
     g = Graph()
     for t in generate_triples(n):
         g.add(t)
-    assert len(g) > n * .9
-    matches = g.match(NamedNode("http://example.com/42"), None, None)
-    matches = g.match(None, NamedNode("http://example/terms/42"), None)
-    matches = g.match(None, None, Literal(42))
+    assert len(g) > n * 0.9
+    g.match(NamedNode("http://example.com/42"), None, None)
+    g.match(None, NamedNode("http://example/terms/42"), None)
+    g.match(None, None, Literal(42))
+
 
 def test_iter_10000_triples():
     n = 10000
     g = Graph()
     triples = set()
     for t in generate_triples(n):
         g.add(t)
         triples.add(t)
-    assert len(g) > n * .9
+    assert len(g) > n * 0.9
     for t in g:
         triples.remove(t)
     assert len(triples) == 0
 
+
 # Dataset Tests
 
+
 def test_add_quad():
-    q = Quad(NamedNode("http://example.com/graph"),NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),Literal("Never!"))
+    q = Quad(
+        NamedNode("http://example.com/graph"),
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        Literal("Never!"),
+    )
     ds = Dataset()
     ds.add(q)
     assert q in ds
 
+
 def test_remove_quad():
-    q = Quad(NamedNode("http://example.com/graph"),NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),Literal("Never!"))
+    q = Quad(
+        NamedNode("http://example.com/graph"),
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        Literal("Never!"),
+    )
     ds = Dataset()
     ds.add(q)
     ds.remove(q)
     assert q not in ds
 
+
 def test_ds_len():
     n = 10
     ds = Dataset()
     for q in generate_quads(n):
         ds.add(q)
     assert len(ds) == 10
 
+
 def test_match_ds_sVV_pattern():
-    q = Quad(NamedNode("http://example.com"),
-             NamedNode("http://purl.org/dc/terms/issued"),Literal("Never!"),
-             NamedNode("http://example.com/graph"))
+    q = Quad(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        Literal("Never!"),
+        NamedNode("http://example.com/graph"),
+    )
     ds = Dataset()
     ds.add(q)
     matches = ds.match(subject=NamedNode("http://example.com"))
     assert q in matches
 
+
 def test_match_ds_quad_pattern():
-    q = Quad(NamedNode("http://example.com"),
-             NamedNode("http://purl.org/dc/terms/issued"),Literal("Never!"),
-             NamedNode("http://example.com/graph"))
+    q = Quad(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        Literal("Never!"),
+        NamedNode("http://example.com/graph"),
+    )
     ds = Dataset()
     ds.add(q)
     matches = ds.match(graph="http://example.com/graph")
     assert q in matches
 
+
 def test_add_graph():
-    t = Triple(NamedNode("http://example.com"), NamedNode("http://purl.org/dc/terms/issued"),Literal("Never!"))
+    t = Triple(
+        NamedNode("http://example.com"),
+        NamedNode("http://purl.org/dc/terms/issued"),
+        Literal("Never!"),
+    )
     g = Graph("http://example.com/graph")
     g.add(t)
     ds = Dataset()
     ds.add_graph(g)
     assert t in ds
 
+
 def generate_quads(n):
     for i in range(n):
-        yield Quad(NamedNode("http://example/" + str(random.randint(1,1000))),
-                   NamedNode("http://purl.org/dc/terms/" + str(random.randint(1,100))),
-                   Literal(random.randint(1,1000)),
-                   NamedNode("http://example/graph/"+str(random.randint(1,1000))))
+        yield Quad(
+            NamedNode("http://example/" + str(random.randint(1, 1000))),
+            NamedNode("http://purl.org/dc/terms/" + str(random.randint(1, 100))),
+            Literal(random.randint(1, 1000)),
+            NamedNode("http://example/graph/" + str(random.randint(1, 1000))),
+        )
+
 
 def test_10000_quads():
     n = 10000
     ds = Dataset()
     for q in generate_quads(n):
         ds.add(q)
-    assert len(ds) > n * .9
-    matches = ds.match(subject=NamedNode("http://example.com/42"),
-                       graph=NamedNode("http://example/graph/42"))
+    assert len(ds) > n * 0.9
+    ds.match(
+        subject=NamedNode("http://example.com/42"),
+        graph=NamedNode("http://example/graph/42"),
+    )
+
 
 def test_iter_10000_quads():
     n = 10000
     ds = Dataset()
     quads = set()
     for q in generate_quads(n):
         ds.add(q)
         quads.add(q)
-    assert len(ds) > n * .9
+    assert len(ds) > n * 0.9
     for quad in ds:
         quads.remove(quad)
     assert len(quads) == 0
 
+
 def test_interfaceName():
     assert Literal("Bob", "en").interfaceName == "Literal"
     assert NamedNode().interfaceName == "NamedNode"
 
+
 def test_BlankNode_id():
     b1 = BlankNode()
     b2 = BlankNode()
     assert b1.value != b2.value
```

### Comparing `pymantic-0.3.0/pymantic/tests/test_turtle.py` & `pymantic-1.0.0/tests/test_turtle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,130 @@
 import os.path
-from pymantic.compat.moves.urllib.parse import urljoin
-import unittest
-from pymantic.parsers import turtle_parser, ntriples_parser
+import pytest
+from urllib.parse import urljoin
+
+from pymantic.parsers import ntriples_parser, turtle_parser
 import pymantic.rdf as rdf
-from pymantic.compat import text_type
 
-turtle_tests_url =\
-    'http://www.w3.org/2013/TurtleTests/'
+turtle_tests_url = "http://www.w3.org/2013/TurtleTests/"
 
 prefixes = {
-    'mf': 'http://www.w3.org/2001/sw/DataAccess/tests/test-manifest#',
-    'qt': 'http://www.w3.org/2001/sw/DataAccess/tests/test-query#',
-    'rdft': 'http://www.w3.org/ns/rdftest#',
+    "mf": "http://www.w3.org/2001/sw/DataAccess/tests/test-manifest#",
+    "qt": "http://www.w3.org/2001/sw/DataAccess/tests/test-query#",
+    "rdft": "http://www.w3.org/ns/rdftest#",
 }
 
 
 def isomorph_triple(triple):
-    from pymantic.primitives import (
-        BlankNode,
-        Literal,
-        NamedNode,
-    )
+    from pymantic.primitives import BlankNode, Literal, NamedNode
 
     if isinstance(triple.subject, BlankNode):
         triple = triple._replace(subject=None)
     if isinstance(triple.object, BlankNode):
         triple = triple._replace(object=None)
     if isinstance(triple.object, Literal) and triple.object.datatype is None:
-        triple = triple._replace(object=triple.object._replace(
-            datatype=NamedNode('http://www.w3.org/2001/XMLSchema#string')))
+        triple = triple._replace(
+            object=triple.object._replace(
+                datatype=NamedNode("http://www.w3.org/2001/XMLSchema#string")
+            )
+        )
 
     return triple
 
 
 def isomorph(graph):
-    return {
-        isomorph_triple(t) for t in graph._triples
-    }
+    return {isomorph_triple(t) for t in graph._triples}
 
 
-@rdf.register_class('mf:Manifest')
+@rdf.register_class("mf:Manifest")
 class Manifest(rdf.Resource):
     prefixes = prefixes
 
-    scalars = frozenset(('rdfs:comment', 'mf:entries'))
+    scalars = frozenset(("rdfs:comment", "mf:entries"))
 
 
-@rdf.register_class('rdft:TestTurtleEval')
-class TestTurtleEval(rdf.Resource):
+@rdf.register_class("rdft:TestTurtleEval")
+class TurtleEvalTest(rdf.Resource):
     prefixes = prefixes
 
-    scalars = frozenset(('mf:name', 'rdfs:comment', 'mf:action', 'mf:result'))
+    scalars = frozenset(("mf:name", "rdfs:comment", "mf:action", "mf:result"))
 
-    def execute(self, test_case):
-        with open(text_type(self['mf:action']), 'rb') as f:
+    def execute(self):
+        with open(str(self["mf:action"]), "rb") as f:
             in_data = f.read()
 
-        with open(text_type(self['mf:result']), 'rb') as f:
+        with open(str(self["mf:result"]), "rb") as f:
             compare_data = f.read()
 
-        base = urljoin(turtle_tests_url,
-                       os.path.basename(text_type(self['mf:action'])))
+        base = urljoin(turtle_tests_url, os.path.basename(str(self["mf:action"])))
 
         test_graph = turtle_parser.parse(in_data, base=base)
         compare_graph = ntriples_parser.parse_string(compare_data)
-        test_case.assertEqual(
-            isomorph(test_graph),
-            isomorph(compare_graph),
-        )
+        assert isomorph(test_graph) == isomorph(compare_graph), self[
+            "rdfs:comment"
+        ].value
 
 
-@rdf.register_class('rdft:TestTurtlePositiveSyntax')
-class TestTurtlePositiveSyntax(rdf.Resource):
+@rdf.register_class("rdft:TestTurtlePositiveSyntax")
+class TurtlePositiveSyntaxTest(rdf.Resource):
     prefixes = prefixes
 
-    scalars = frozenset(('mf:name', 'rdfs:comment', 'mf:action'))
+    scalars = frozenset(("mf:name", "rdfs:comment", "mf:action"))
 
-    def execute(self, test_case):
-        with open(text_type(self['mf:action']), 'rb') as f:
+    def execute(self):
+        with open(str(self["mf:action"]), "rb") as f:
             in_data = f.read()
 
-        base = urljoin(turtle_tests_url,
-                       os.path.basename(text_type(self['mf:action'])))
-        test_graph = turtle_parser.parse(in_data, base=base)
+        base = urljoin(turtle_tests_url, os.path.basename(str(self["mf:action"])))
+        turtle_parser.parse(in_data, base=base)
 
 
-@rdf.register_class('rdft:TestTurtleNegativeSyntax')
-class TestTurtleNegativeSyntax(rdf.Resource):
+@rdf.register_class("rdft:TestTurtleNegativeSyntax")
+class TurtleNegativeSyntaxTest(rdf.Resource):
     prefixes = prefixes
 
-    scalars = frozenset(('mf:name', 'rdfs:comment', 'mf:action'))
+    scalars = frozenset(("mf:name", "rdfs:comment", "mf:action"))
 
-    def execute(self, test_case):
-        with open(text_type(self['mf:action']), 'rb') as f:
+    def execute(self):
+        with open(str(self["mf:action"]), "rb") as f:
             in_data = f.read()
 
-        base = urljoin(turtle_tests_url,
-                       os.path.basename(text_type(self['mf:action'])))
-        with test_case.assertRaises(Exception):
+        base = urljoin(turtle_tests_url, os.path.basename(str(self["mf:action"])))
+        with pytest.raises(Exception):
             turtle_parser.parse(in_data, base=base)
 
 
-@rdf.register_class('rdft:TestTurtleNegativeEval')
-class TestTurtleNegativeEval(rdf.Resource):
+@rdf.register_class("rdft:TestTurtleNegativeEval")
+class TurtleNegativeEvalTest(rdf.Resource):
     prefixes = prefixes
 
-    scalars = frozenset(('mf:name', 'rdfs:comment', 'mf:action'))
+    scalars = frozenset(("mf:name", "rdfs:comment", "mf:action"))
 
-    def execute(self, test_case):
-        with open(text_type(self['mf:action']), 'rb') as f:
+    def execute(self):
+        with open(str(self["mf:action"]), "rb") as f:
             in_data = f.read()
 
-        base = urljoin(turtle_tests_url,
-                       os.path.basename(text_type(self['mf:action'])))
-        with test_case.assertRaises(Exception):
+        base = urljoin(turtle_tests_url, os.path.basename(str(self["mf:action"])))
+        with pytest.raises(Exception):
             turtle_parser.parse(in_data, base=base)
 
 
-base = os.path.join(os.path.dirname(__file__), 'TurtleTests/')
+base = os.path.join(os.path.dirname(__file__), "TurtleTests/")
 
-manifest_name = os.path.join(base, 'manifest.ttl')
+manifest_name = os.path.join(base, "manifest.ttl")
 
-with open(manifest_name, 'rb') as f:
+with open(manifest_name, "rb") as f:
     manifest_turtle = f.read()
 
 manifest_graph = turtle_parser.parse(manifest_turtle, base=base)
 
 manifest = Manifest(manifest_graph, base)
 
-
-class TurtleTests(unittest.TestCase):
-    @classmethod
-    def _make_test_case(cls, test_case):
-        def test_method(self):
-            return test_case.execute(self)
-
-        test_name = 'test_' + test_case['mf:name'].value.replace('-', '_')
-        test_method.__name__ = str(test_name)
-        test_method.func_name = test_name.encode('utf8')
-        test_method.func_doc = u'{} ({})'.format(
-            test_case['rdfs:comment'].value,
-            test_name,
-        )
-        setattr(cls, test_name, test_method)
+turtle_test_cases = {
+    test_case["mf:name"].value: test_case
+    for test_case in manifest["mf:entries"].as_(rdf.List)
+}
 
 
-for test_case in list(manifest['mf:entries'].as_(rdf.List)):
-    TurtleTests._make_test_case(test_case)
+@pytest.mark.parametrize(["turtle_test_case_name"], zip(turtle_test_cases.keys()))
+def test_turtle(turtle_test_case_name):
+    turtle_test_cases[turtle_test_case_name].execute()
```

### Comparing `pymantic-0.3.0/pymantic/tests/test_util.py` & `pymantic-1.0.0/tests/test_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from nose.tools import *
-from pymantic.util import *
+from pymantic.util import normalize_iri, quote_normalized_iri
+
 
 def test_normalize_iri_no_escapes():
-    uri = 'http://example.com/foo/bar?garply=aap&maz=bies'
+    uri = "http://example.com/foo/bar?garply=aap&maz=bies"
     normalized = normalize_iri(uri)
-    assert normalized == u'http://example.com/foo/bar?garply=aap&maz=bies'
+    assert normalized == "http://example.com/foo/bar?garply=aap&maz=bies"
     assert normalized == normalize_iri(normalized)
     assert quote_normalized_iri(normalized) == uri
 
+
 def test_normalize_iri_escaped_slash():
-    uri = 'http://example.com/foo%2Fbar?garply=aap&maz=bies'
+    uri = "http://example.com/foo%2Fbar?garply=aap&maz=bies"
     normalized = normalize_iri(uri)
-    assert normalized == u'http://example.com/foo%2Fbar?garply=aap&maz=bies'
+    assert normalized == "http://example.com/foo%2Fbar?garply=aap&maz=bies"
     assert normalized == normalize_iri(normalized)
     assert quote_normalized_iri(normalized) == uri
 
+
 def test_normalize_iri_escaped_ampersand():
-    uri = 'http://example.com/foo/bar?garply=aap%26yak&maz=bies'
+    uri = "http://example.com/foo/bar?garply=aap%26yak&maz=bies"
     normalized = normalize_iri(uri)
-    assert normalized == u'http://example.com/foo/bar?garply=aap%26yak&maz=bies'
+    assert normalized == "http://example.com/foo/bar?garply=aap%26yak&maz=bies"
     assert normalized == normalize_iri(normalized)
     assert quote_normalized_iri(normalized) == uri
 
+
 def test_normalize_iri_escaped_international():
-    uri = 'http://example.com/foo/bar?garply=aap&maz=bi%C3%89s'
+    uri = "http://example.com/foo/bar?garply=aap&maz=bi%C3%89s"
     normalized = normalize_iri(uri)
-    assert normalized == u'http://example.com/foo/bar?garply=aap&maz=bi\u00C9s'
+    assert normalized == "http://example.com/foo/bar?garply=aap&maz=bi\u00C9s"
     assert normalized == normalize_iri(normalized)
     assert quote_normalized_iri(normalized) == uri
```

### Comparing `pymantic-0.3.0/pymantic/util.py` & `pymantic-1.0.0/src/pymantic/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,143 @@
 """Utility functions used throughout pymantic."""
 
-__all__ = ['en', 'de', 'one_or_none', 'normalize_iri', 'quote_normalized_iri',]
+__all__ = ["en", "de", "one_or_none", "normalize_iri", "quote_normalized_iri"]
 
 import re
-from .compat.moves.urllib.parse import quote
-from .compat import int2byte
+from urllib.parse import quote
+
 
 def en(value):
     """Returns an RDF literal from the en language for the given value."""
     from pymantic.primitives import Literal
-    return Literal(value, language='en')
+
+    return Literal(value, language="en")
+
 
 def de(value):
     """Returns an RDF literal from the de language for the given value."""
     from pymantic.primitives import Literal
-    return Literal(value, language='de')
+
+    return Literal(value, language="de")
+
 
 def one_or_none(values):
     """Fetch the first value from values, or None if values is empty. Raises
     ValueError if values has more than one thing in it."""
     if not values:
         return None
     if len(values) > 1:
-        raise ValueError('Got more than one value.')
+        raise ValueError("Got more than one value.")
     return values[0]
 
-percent_encoding_re = re.compile(r'(?:%(?![01][0-9a-fA-F])(?!20)[a-fA-F0-9][a-fA-F0-9])+')
 
-reserved_in_iri = ["%", ":", "/", "?", "#", "[", "]", "@", "!", "$", "&", "'",\
-                   "(", ")", "*", "+", ",", ";", "="]
+percent_encoding_re = re.compile(
+    r"(?:%(?![01][0-9a-fA-F])(?!20)[a-fA-F0-9][a-fA-F0-9])+"
+)
+
+reserved_in_iri = [
+    "%",
+    ":",
+    "/",
+    "?",
+    "#",
+    "[",
+    "]",
+    "@",
+    "!",
+    "$",
+    "&",
+    "'",
+    "(",
+    ")",
+    "*",
+    "+",
+    ",",
+    ";",
+    "=",
+]
+
 
 def percent_decode(regmatch):
-    encoded = b''
-    for group in regmatch.group(0)[1:].split('%'):
-        encoded += int2byte(int(group, 16))
-    uni = encoded.decode('utf-8')
+    encoded = b""
+    for group in regmatch.group(0)[1:].split("%"):
+        encoded += int(group, 16).to_bytes(1, "big")
+    uni = encoded.decode("utf-8")
     for res in reserved_in_iri:
-        uni = uni.replace(res, '%%%02X' % ord(res))
+        uni = uni.replace(res, "%%%02X" % ord(res))
     return uni
 
+
 def normalize_iri(iri):
     """Normalize an IRI using the Case Normalization (5.3.2.1) and
     Percent-Encoding Normalization (5.3.2.3) from RFC 3987. The IRI should be a
     unicode object."""
 
     return percent_encoding_re.sub(percent_decode, iri)
 
+
 def percent_encode(char):
-    from .compat import ordbyte
+    return "".join("%%%02X" % char for char in char.encode("utf-8"))
 
-    return ''.join('%%%02X' % ordbyte(char) for char in char.encode('utf-8'))
 
 def quote_normalized_iri(normalized_iri):
     """Percent-encode a normalized IRI; IE, all reserved characters are presumed
     to be themselves and not percent encoded. All other unsafe characters are
     percent-encoded."""
-    normalized_uri = ''.join(percent_encode(char) if ord(char) > 127 else char for\
-                             char in normalized_iri)
-    return quote(normalized_uri, safe=''.join(reserved_in_iri))
+    normalized_uri = "".join(
+        percent_encode(char) if ord(char) > 127 else char for char in normalized_iri
+    )
+    return quote(normalized_uri, safe="".join(reserved_in_iri))
 
 
 def smart_urljoin(base, url):
     """urljoin, only an empty fragment from the relative(?) URL will be
     preserved.
     """
-    from .compat.moves.urllib.parse import urljoin
+    from urllib.parse import urljoin
 
     joined = urljoin(base, url)
-    if url.endswith('#') and not joined.endswith('#'):
-        joined += '#'
+    if url.endswith("#") and not joined.endswith("#"):
+        joined += "#"
     return joined
 
 
 def grouper(iterable, n, fillvalue=None):
     "Collect data into fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, 'x') --> ABC DEF Gxx"
 
-    from .compat.moves import zip_longest
+    from itertools import zip_longest
+
     args = [iter(iterable)] * n
     return zip_longest(*args, fillvalue=fillvalue)
 
 
 ESCAPE_MAP = {
-    't': '\t',
-    'b': '\b',
-    'n': '\n',
-    'r': '\r',
-    'f': '\f',
-    '"': '\"',
-    "'": "\'",
+    "t": "\t",
+    "b": "\b",
+    "n": "\n",
+    "r": "\r",
+    "f": "\f",
+    '"': '"',
+    "'": "'",
     "\\": "\\",
 }
 
 
-ECHAR_MAP = {
-    v: '\\' + k for k, v in ESCAPE_MAP.items()
-}
+ECHAR_MAP = {v: "\\" + k for k, v in ESCAPE_MAP.items()}
 
 
 def process_escape(escape):
-    from .compat import unichr
-
     escape = escape.group(0)[1:]
 
-    if escape[0] in ('u', 'U'):
-        return unichr(int(escape[1:], 16))
+    if escape[0] in ("u", "U"):
+        return chr(int(escape[1:], 16))
     else:
         return ESCAPE_MAP.get(escape[0], escape[0])
 
 
 def decode_literal(literal):
     return re.sub(
-        r'\\u[a-fA-F0-9]{4}|\\U[a-fA-F0-9]{8}|\\[^uU]',
+        r"\\u[a-fA-F0-9]{4}|\\U[a-fA-F0-9]{8}|\\[^uU]",
         process_escape,
         literal,
     )
```

### Comparing `pymantic-0.3.0/pymantic.egg-info/PKG-INFO` & `pymantic-1.0.0/src/pymantic.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: pymantic
-Version: 0.3.0
+Version: 1.0.0
 Summary: Semantic Web and RDF library for Python
 Home-page: https://github.com/norcalrdf/pymantic/
 Author: Gavin Carothers, Nick Pilon
 Author-email: gavin@carothers.name, npilon@gmail.com
 License: BSD
-Description: ========
-        Pymantic
-        ========
-        ---------------------------------------
-        Semantic Web and RDF library for Python
-        ---------------------------------------
-        
-        
-        Quick Start
-        ===========
-        ::
-        
-            >>> from pymantic.rdf import *
-            >>> from pymantic.parsers import turtle_parser
-            >>> import requests
-            >>> Resource.prefixes['foaf'] = Prefix('http://xmlns.com/foaf/0.1/')
-            >>> graph = turtle_parser.parse(requests.get('https://raw.github.com/norcalrdf/pymantic/master/examples/foaf-bond.ttl').text)
-            >>> bond_james = Resource(graph, 'http://example.org/stuff/Bond')
-            >>> print("%s knows:" % (bond_james.get_scalar('foaf:name'),))
-            >>> for person in bond_james['foaf:knows']:
-                    print(person.get_scalar('foaf:name'))
-        
-        
-        
-        Requirements
-        ============
-        
-        ``pymantic`` requires Python 3.6 or higher.
-        ``lark`` is used for the Turtle and NTriples parser.
-        The ``requests`` library is used for HTTP requests and the SPARQL client.
-        ``lxml`` and ``rdflib`` are required by the SPARQL client as well.
-        
-        
-        Install
-        =======
-        
-        ::
-        
-            $ pip install pymantic
-        
-        This will install ``pymantic`` and all its dependencies.
-        
-        
-        Documentation
-        =============
-        
-        Generating a local copy of the documentation requires Sphinx:
-        
-        ::
-        
-            $ pip install Sphinx
-        
-        
-        
-Keywords: RDF N3 Turtle Semantics Web3.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Keywords: RDF N3 Turtle Semantics
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Markup
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
+License-File: LICENSE
+
+========
+Pymantic
+========
+---------------------------------------
+Semantic Web and RDF library for Python
+---------------------------------------
+
+
+Quick Start
+===========
+::
+
+    >>> from pymantic.rdf import *
+    >>> from pymantic.parsers import turtle_parser
+    >>> import requests
+    >>> Resource.prefixes['foaf'] = Prefix('http://xmlns.com/foaf/0.1/')
+    >>> graph = turtle_parser.parse(requests.get('https://raw.github.com/norcalrdf/pymantic/master/examples/foaf-bond.ttl').text)
+    >>> bond_james = Resource(graph, 'http://example.org/stuff/Bond')
+    >>> print("%s knows:" % (bond_james.get_scalar('foaf:name'),))
+    >>> for person in bond_james['foaf:knows']:
+            print(person.get_scalar('foaf:name'))
+
+
+
+Requirements
+============
+
+``pymantic`` requires Python 3.9 or higher.
+``lark`` is used for the Turtle and NTriples parser.
+The ``requests`` library is used for HTTP requests and the SPARQL client.
+``lxml`` and ``rdflib`` are required by the SPARQL client as well.
+
+
+Install
+=======
+
+::
+
+    $ pip install pymantic
+
+This will install ``pymantic`` and all its dependencies.
+
+
+Documentation
+=============
+
+Generating a local copy of the documentation requires Sphinx:
+
+::
+
+    $ pip install Sphinx
+
+
```

### Comparing `pymantic-0.3.0/pymantic.egg-info/SOURCES.txt` & `pymantic-1.0.0/src/pymantic.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,36 @@
+LICENSE
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
-pymantic/__init__.py
-pymantic/change_tracking.py
-pymantic/compat.py
-pymantic/primitives.py
-pymantic/rdf.py
-pymantic/serializers.py
-pymantic/sparql.py
-pymantic/uri_schemes.py
-pymantic/util.py
-pymantic.egg-info/PKG-INFO
-pymantic.egg-info/SOURCES.txt
-pymantic.egg-info/dependency_links.txt
-pymantic.egg-info/entry_points.txt
-pymantic.egg-info/not-zip-safe
-pymantic.egg-info/requires.txt
-pymantic.egg-info/top_level.txt
-pymantic/parsers/__init__.py
-pymantic/parsers/base.py
-pymantic/parsers/jsonld.py
-pymantic/parsers/rdfxml.py
-pymantic/parsers/lark/__init__.py
-pymantic/parsers/lark/base.py
-pymantic/parsers/lark/nquads.py
-pymantic/parsers/lark/ntriples.py
-pymantic/parsers/lark/turtle.py
-pymantic/scripts/__init__.py
-pymantic/scripts/bnf2html
-pymantic/scripts/named_graph_to_nquads
-pymantic/tests/__init__.py
-pymantic/tests/test_RDF.py
-pymantic/tests/test_SPARQL.py
-pymantic/tests/test_parsers.py
-pymantic/tests/test_primitives.py
-pymantic/tests/test_serializers.py
-pymantic/tests/test_turtle.py
-pymantic/tests/test_util.py
-pymantic/vocab/__init__.py
-pymantic/vocab/skos.py
+src/pymantic/__init__.py
+src/pymantic/primitives.py
+src/pymantic/rdf.py
+src/pymantic/serializers.py
+src/pymantic/sparql.py
+src/pymantic/uri_schemes.py
+src/pymantic/util.py
+src/pymantic.egg-info/PKG-INFO
+src/pymantic.egg-info/SOURCES.txt
+src/pymantic.egg-info/dependency_links.txt
+src/pymantic.egg-info/requires.txt
+src/pymantic.egg-info/top_level.txt
+src/pymantic.egg-info/zip-safe
+src/pymantic/parsers/__init__.py
+src/pymantic/parsers/base.py
+src/pymantic/parsers/jsonld.py
+src/pymantic/parsers/rdfxml.py
+src/pymantic/parsers/lark/__init__.py
+src/pymantic/parsers/lark/base.py
+src/pymantic/parsers/lark/nquads.py
+src/pymantic/parsers/lark/ntriples.py
+src/pymantic/parsers/lark/turtle.py
+src/pymantic/scripts/__init__.py
+src/pymantic/vocab/__init__.py
+src/pymantic/vocab/skos.py
+tests/test_RDF.py
+tests/test_SPARQL.py
+tests/test_parsers.py
+tests/test_primitives.py
+tests/test_serializers.py
+tests/test_turtle.py
+tests/test_util.py
```

