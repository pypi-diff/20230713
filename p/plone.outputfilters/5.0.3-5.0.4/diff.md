# Comparing `tmp/plone.outputfilters-5.0.3.tar.gz` & `tmp/plone.outputfilters-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.outputfilters-5.0.3.tar", last modified: Fri Jun 16 16:59:00 2023, max compression
+gzip compressed data, was "plone.outputfilters-5.0.4.tar", last modified: Thu Jul 13 21:51:02 2023, max compression
```

## Comparing `plone.outputfilters-5.0.3.tar` & `plone.outputfilters-5.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.796342 plone.outputfilters-5.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)     8920 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    16193 2023-06-16 16:59:00.796514 plone.outputfilters-5.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.783681 plone.outputfilters-5.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      736 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.783992 plone.outputfilters-5.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.789606 plone.outputfilters-5.0.3/plone/outputfilters/
--rw-r--r--   0 maurits    (501) staff       (20)     2752 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.791051 plone.outputfilters-5.0.3/plone/outputfilters/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      240 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/captioned_image.pt
--rw-r--r--   0 maurits    (501) staff       (20)      326 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/captioned_image.py
--rw-r--r--   0 maurits    (501) staff       (20)      472 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2283 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/browser/resolveuid.py
--rw-r--r--   0 maurits    (501) staff       (20)      788 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.792611 plone.outputfilters-5.0.3/plone/outputfilters/filters/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      865 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      373 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1721 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/filters/resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)      744 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/mimetype.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.779625 plone.outputfilters-5.0.3/plone/outputfilters/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.793070 plone.outputfilters-5.0.3/plone/outputfilters/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/profiles/default/plone.outputfilters.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.795135 plone.outputfilters-5.0.3/plone/outputfilters/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_apply_filters.py
--rw-r--r--   0 maurits    (501) staff       (20)      787 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_picture_variants.py
--rw-r--r--   0 maurits    (501) staff       (20)    27360 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_resolveuid_and_caption.py
--rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/tests/test_transforms.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.796110 plone.outputfilters-5.0.3/plone/outputfilters/transforms/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:59:00.786839 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    16193 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      325 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/plone.outputfilters.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1717 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-06-16 16:59:00.797095 plone.outputfilters-5.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-06-16 16:59:00.000000 plone.outputfilters-5.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.533859 plone.outputfilters-5.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)     9141 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    16414 2023-07-13 21:51:02.533540 plone.outputfilters-5.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.520303 plone.outputfilters-5.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.520722 plone.outputfilters-5.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.525684 plone.outputfilters-5.0.4/plone/outputfilters/
+-rw-r--r--   0 maurits    (501) staff       (20)     2752 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      252 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.527358 plone.outputfilters-5.0.4/plone/outputfilters/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/browser/captioned_image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      326 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/browser/captioned_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)      472 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2283 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/browser/resolveuid.py
+-rw-r--r--   0 maurits    (501) staff       (20)      788 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.529228 plone.outputfilters-5.0.4/plone/outputfilters/filters/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/filters/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/filters/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      373 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/filters/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1813 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/filters/picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13893 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/filters/resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)      744 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/mimetype.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.517438 plone.outputfilters-5.0.4/plone/outputfilters/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.529631 plone.outputfilters-5.0.4/plone/outputfilters/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/profiles/default/plone.outputfilters.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1604 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.531930 plone.outputfilters-5.0.4/plone/outputfilters/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19200 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/test_apply_filters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      787 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11184 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/test_picture_variants.py
+-rw-r--r--   0 maurits    (501) staff       (20)    27360 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/test_resolveuid_and_caption.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2240 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/tests/test_transforms.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.533128 plone.outputfilters-5.0.4/plone/outputfilters/transforms/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/transforms/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1210 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:51:02.523476 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    16414 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1708 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      325 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-13 21:51:02.000000 plone.outputfilters-5.0.4/plone.outputfilters.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3828 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-13 21:51:02.534029 plone.outputfilters-5.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2533 2023-07-13 21:51:01.000000 plone.outputfilters-5.0.4/setup.py
```

### Comparing `plone.outputfilters-5.0.3/CHANGES.rst` & `plone.outputfilters-5.0.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-07-13)
+------------------
+
+Bug fixes:
+
+
+- Call registry once per filter rather than for each img tag.
+  [gotcha] (less_call_to_registry)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 5.0.3 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
```

### Comparing `plone.outputfilters-5.0.3/PKG-INFO` & `plone.outputfilters-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.3
+Version: 5.0.4
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-07-13)
+------------------
+
+Bug fixes:
+
+
+- Call registry once per filter rather than for each img tag.
+  [gotcha] (less_call_to_registry)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 5.0.3 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
```

### Comparing `plone.outputfilters-5.0.3/README.rst` & `plone.outputfilters-5.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/docs/LICENSE.GPL` & `plone.outputfilters-5.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/docs/LICENSE.txt` & `plone.outputfilters-5.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/README.rst` & `plone.outputfilters-5.0.4/plone/outputfilters/README.rst`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/browser/resolveuid.py` & `plone.outputfilters-5.0.4/plone/outputfilters/browser/resolveuid.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/configure.zcml` & `plone.outputfilters-5.0.4/plone/outputfilters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/filters/configure.zcml` & `plone.outputfilters-5.0.4/plone/outputfilters/filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/filters/picture_variants.py` & `plone.outputfilters-5.0.4/plone/outputfilters/filters/picture_variants.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,26 @@
         return self.context is not None
 
     def __init__(self, context=None, request=None):
         self.current_status = None
         self.context = context
         self.request = request
         self.img2picturetag = Img2PictureTag()
+        self.all_picture_variants = get_picture_variants()
 
     def __call__(self, data):
         soup = BeautifulSoup(safe_text(data), "html.parser")
 
         for elem in soup.find_all("img"):
             picture_variant_name = elem.attrs.get("data-picturevariant", "")
             if not picture_variant_name:
                 continue
-            picture_variants_config = get_picture_variants().get(picture_variant_name)
+            picture_variants_config = self.all_picture_variants.get(
+                picture_variant_name
+            )
             if not picture_variants_config:
                 logger.warning(
                     "Could not find the given picture_variant_name {}, leave tag untouched!".format(
                         picture_variant_name
                     )
                 )
                 continue
```

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/filters/resolveuid_and_caption.py` & `plone.outputfilters-5.0.4/plone/outputfilters/filters/resolveuid_and_caption.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/interfaces.py` & `plone.outputfilters-5.0.4/plone/outputfilters/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/setuphandlers.py` & `plone.outputfilters-5.0.4/plone/outputfilters/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/testing.py` & `plone.outputfilters-5.0.4/plone/outputfilters/testing.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/image.jpg` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_apply_filters.py` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/test_apply_filters.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_docs.py` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_picture_variants.py` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/test_picture_variants.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_resolveuid_and_caption.py` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/test_resolveuid_and_caption.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/tests/test_transforms.py` & `plone.outputfilters-5.0.4/plone/outputfilters/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py` & `plone.outputfilters-5.0.4/plone/outputfilters/transforms/html_to_plone_outputfilters_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py` & `plone.outputfilters-5.0.4/plone/outputfilters/transforms/plone_outputfilters_html_to_html.py`

 * *Files identical despite different names*

### Comparing `plone.outputfilters-5.0.3/plone.outputfilters.egg-info/PKG-INFO` & `plone.outputfilters-5.0.4/plone.outputfilters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.outputfilters
-Version: 5.0.3
+Version: 5.0.4
 Summary: Transformations applied to HTML in Plone text fields as they are rendered
 Home-page: http://github.com/plone/plone.outputfilters
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL
 Keywords: plone transform filter uid caption
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-07-13)
+------------------
+
+Bug fixes:
+
+
+- Call registry once per filter rather than for each img tag.
+  [gotcha] (less_call_to_registry)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 5.0.3 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Return a 404 Not Found response if the resolveuid view is called with no uuid. @davisagli (#43)
```

### Comparing `plone.outputfilters-5.0.3/plone.outputfilters.egg-info/SOURCES.txt` & `plone.outputfilters-5.0.4/plone.outputfilters.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.outputfilters.egg-info/PKG-INFO
 plone.outputfilters.egg-info/SOURCES.txt
 plone.outputfilters.egg-info/dependency_links.txt
```

### Comparing `plone.outputfilters-5.0.3/setup.py` & `plone.outputfilters-5.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "5.0.3"
+version = "5.0.4"
 
 
 def read(filename):
     with open(filename) as myfile:
         try:
             return myfile.read()
         except UnicodeDecodeError:
```

