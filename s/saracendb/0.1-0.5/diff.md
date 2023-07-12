# Comparing `tmp/saracendb-0.1.tar.gz` & `tmp/saracendb-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracendb-0.1.tar", last modified: Tue Jul 11 15:08:45 2023, max compression
+gzip compressed data, was "saracendb-0.5.tar", last modified: Wed Jul 12 22:33:13 2023, max compression
```

## Comparing `saracendb-0.1.tar` & `saracendb-0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.712320 saracendb-0.1/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.712176 saracendb-0.1/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      125 2023-07-11 14:51:10.000000 saracendb-0.1/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711159 saracendb-0.1/saracendb/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 14:52:10.000000 saracendb-0.1/saracendb/__init__.py
--rw-r--r--   0 richardkammermeier   (501) staff       (20)     1674 2023-07-11 14:51:30.000000 saracendb-0.1/saracendb/main.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-11 15:08:45.711967 saracendb-0.1/saracendb.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      552 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      222 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        8 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-11 15:08:45.000000 saracendb-0.1/saracendb.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-11 15:08:45.712364 saracendb-0.1/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      914 2023-07-11 15:06:06.000000 saracendb-0.1/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.347429 saracendb-0.5/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     2341 2023-07-12 22:33:13.347304 saracendb-0.5/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     1914 2023-07-11 15:57:26.000000 saracendb-0.5/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.346590 saracendb-0.5/saracendb/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     6640 2023-07-12 22:32:27.000000 saracendb-0.5/saracendb/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 22:33:13.347147 saracendb-0.5/saracendb.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)     2341 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      204 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       10 2023-07-12 22:33:13.000000 saracendb-0.5/saracendb.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-12 22:33:13.347468 saracendb-0.5/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      923 2023-07-12 22:32:55.000000 saracendb-0.5/setup.py
```

### Comparing `saracendb-0.1/setup.py` & `saracendb-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1'
+VERSION = '0.5'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracendb",
     version=VERSION,
     author="Saracen Rhue",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pymongo'],
+    install_requires=['pymongo','pyyaml'],
     keywords=['python', 'db'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

