# Comparing `tmp/saracendb-0.5.tar.gz` & `tmp/saracendb-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.5.tar", last modified: Wed Jul 12 22:33:13 2023, max compression
+gzip compressed data, was "saracendb-0.6.tar", last modified: Thu Jul 13 14:50:13 2023, max compression
```

## Comparing `saracendb-0.5.tar` & `saracendb-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.347429 saracendb-0.5/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     2341 2023-07-12 22:33:13.347304 saracendb-0.5/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1914 2023-07-11 15:57:26.000000 saracendb-0.5/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.346590 saracendb-0.5/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     6640 2023-07-12 22:32:27.000000 saracendb-0.5/saracendb/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.347147 saracendb-0.5/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     2341 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-12 22:33:13.347468 saracendb-0.5/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-12 22:32:55.000000 saracendb-0.5/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.981534 saracendb-0.6/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-13 14:50:13.981395 saracendb-0.6/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4107 2023-07-12 23:26:35.000000 saracendb-0.6/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.980507 saracendb-0.6/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)    10942 2023-07-13 14:47:19.000000 saracendb-0.6/saracendb/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-13 14:50:13.981212 saracendb-0.6/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     4534 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-13 14:50:13.000000 saracendb-0.6/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-13 14:50:13.981576 saracendb-0.6/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-13 14:47:32.000000 saracendb-0.6/setup.py
```

### Comparing `saracendb-0.5/setup.py` & `saracendb-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.5'
+VERSION = '0.6'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
```

