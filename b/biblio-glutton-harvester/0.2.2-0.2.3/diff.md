# Comparing `tmp/biblio_glutton_harvester-0.2.2.tar.gz` & `tmp/biblio_glutton_harvester-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblio_glutton_harvester-0.2.2.tar", last modified: Thu Jul  6 19:27:56 2023, max compression
+gzip compressed data, was "biblio_glutton_harvester-0.2.3.tar", last modified: Thu Jul 13 18:38:30 2023, max compression
```

## Comparing `biblio_glutton_harvester-0.2.2.tar` & `biblio_glutton_harvester-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 19:27:56.524746 biblio_glutton_harvester-0.2.2/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-07-06 10:18:15.000000 biblio_glutton_harvester-0.2.2/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 19:27:56.524746 biblio_glutton_harvester-0.2.2/PKG-INFO
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-06 19:27:56.524746 biblio_glutton_harvester-0.2.2/biblio_glutton_harvester.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-06 19:27:56.000000 biblio_glutton_harvester-0.2.2/biblio_glutton_harvester.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      208 2023-07-06 19:27:56.000000 biblio_glutton_harvester-0.2.2/biblio_glutton_harvester.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 19:27:56.000000 biblio_glutton_harvester-0.2.2/biblio_glutton_harvester.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-06 19:27:56.000000 biblio_glutton_harvester-0.2.2/biblio_glutton_harvester.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-06 19:27:56.524746 biblio_glutton_harvester-0.2.2/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      209 2023-07-06 19:27:21.000000 biblio_glutton_harvester-0.2.2/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:38:30.437507 biblio_glutton_harvester-0.2.3/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-07-06 10:18:15.000000 biblio_glutton_harvester-0.2.3/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-13 18:38:30.437507 biblio_glutton_harvester-0.2.3/PKG-INFO
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:38:30.437507 biblio_glutton_harvester-0.2.3/biblio_glutton_harvester.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      174 2023-07-13 18:38:30.000000 biblio_glutton_harvester-0.2.3/biblio_glutton_harvester.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      208 2023-07-13 18:38:30.000000 biblio_glutton_harvester-0.2.3/biblio_glutton_harvester.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:38:30.000000 biblio_glutton_harvester-0.2.3/biblio_glutton_harvester.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:38:30.000000 biblio_glutton_harvester-0.2.3/biblio_glutton_harvester.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 18:38:30.437507 biblio_glutton_harvester-0.2.3/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      209 2023-07-13 18:36:23.000000 biblio_glutton_harvester-0.2.3/setup.py
```

### Comparing `biblio_glutton_harvester-0.2.2/LICENSE` & `biblio_glutton_harvester-0.2.3/LICENSE`

 * *Files identical despite different names*

