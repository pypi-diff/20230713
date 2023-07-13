# Comparing `tmp/nics-2.7.2.tar.gz` & `tmp/nics-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-5ypn0xps/nics-2.7.2.tar", last modified: Sat Jul  8 14:19:50 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-o5_si_i4/nics-2.8.1.tar", last modified: Thu Jul 13 07:02:44 2023, max compression
```

## Comparing `nics-2.7.2.tar` & `nics-2.8.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 14:19:43.000000 nics-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 14:19:43.000000 nics-2.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 14:19:50.000000 nics-2.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-08 14:19:43.000000 nics-2.7.2/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/baz.md
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/logo200.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-08 14:19:43.000000 nics-2.7.2/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 14:19:50.000000 nics-2.7.2/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-08 14:19:44.000000 nics-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-08 14:19:43.000000 nics-2.7.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 14:19:50.000000 nics-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 14:19:43.000000 nics-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 07:02:33.000000 nics-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 07:02:33.000000 nics-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 07:02:44.000000 nics-2.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 07:02:33.000000 nics-2.8.1/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/docs/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/2 - Pages/baz.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/2 - Pages/logo200.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/docs/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/_sass/main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/_sass/sass-code-highlight.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-13 07:02:33.000000 nics-2.8.1/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 07:02:44.000000 nics-2.8.1/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 07:02:34.000000 nics-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 07:02:33.000000 nics-2.8.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 07:02:44.000000 nics-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 07:02:33.000000 nics-2.8.1/setup.py
```

### Comparing `nics-2.7.2/LICENSE` & `nics-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/__init__.py` & `nics-2.8.1/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/_template/docs/favicon.png` & `nics-2.8.1/nics/main/_template/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/_template/docs/tree/2 - Pages/logo200.png` & `nics-2.8.1/nics/main/_template/docs/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/_template/web/_sass/header.scss` & `nics-2.8.1/nics/main/_template/web/_sass/header.scss`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 header {
     display: flex;
     flex-direction: column;
-    
     margin: 0;
-
     color: hsl($hue-signature, 33%, 7%);
 
     h1 {
         margin: 0;
         margin-top: 0;
         margin-bottom: 37px;
         padding: 13px;
         padding-left: 41px;
     
-        // same color as footer
+        // Same color as footer
         background-color: hsl($hue-signature, 81%, 4%);
         color: hsl($hue-signature, 65%, 91%);
     }
 
     a {
         text-decoration: none;
         color: inherit;
-    }
-    a:hover {
-        text-decoration: underline;
+        &:hover {
+            text-decoration: underline;
+        }
     }
 
     button {
         color: inherit;
     }
 }
 
@@ -53,15 +51,14 @@
     width: 100%;
     padding: 15px;
 
     background-color: hsl($hue-signature, 35%, 76%);
     border: none;
     border-radius: 7px;
 
-    font-family: $font2;
     font-size: 23px;
     text-align: left;
     cursor: pointer;
 }
 
 .main {
     display: flex;
@@ -74,22 +71,20 @@
 
     padding: 9px;
 
     background-color: hsl($hue-signature, 35%, 79%);
     border: none;
     border-radius: 7px;
 
-    font-family: $font2;
     font-size: 17px;
     text-align: left;
     cursor: pointer;
 }
-.main a {
-    font-family: $font2;
-}
+// .main a {
+// }
 
 .child {
     display: none;
     flex-direction: column;
 
     padding: 0 21px;
     gap: 7px;
```

### Comparing `nics-2.7.2/nics/main/_template/web/_sass/main.scss` & `nics-2.8.1/nics/main/_template/web/_sass/main.scss`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,62 @@
 ---
-# Jekyll requires this front matter, including the "#" sign, to convert main.scss to main.css.
 ---
+// Note: Jekyll needs the front matter above to make this file work
+.a4b1e3f8d9 {opacity: 1;}  // This line is intended to silence the error warning message in VS Code
 
 @import url('https://fonts.googleapis.com/css2?family=Caveat&display=swap');
 $font: 'Caveat', cursive;
-@import url('https://fonts.googleapis.com/css2?family=Caveat&family=Grandstander&display=swap');
-$font2: 'Grandstander', cursive;
-// monospace font
-@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono&display=swap');
-$font3: 'IBM Plex Mono', monospace;
 
-$font-size-mobile: 16px;
 $mobile-width: 850px;
 
-@import "constants";  // will be created during compilation
-@import "header";
-@import "footer";
+@import "constants";  // Will be created during compilation
 
 body {
-  
-	// remove the unwanted margin
-	margin: 0;
-
-	// keep showing the scrollbar to prevent glitching
-	overflow-y: scroll;
-
-	background-color: hsl($hue-signature, 15%, 87%);
+	margin: 0;  // Remove the unwanted margin
+    overflow-y: scroll;  // Keep showing the scrollbar to prevent glitching
+	// Main font
+    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
+	// Default page color
+    background-color: hsl($hue-signature, 15%, 91%);;
+    // Default font color
+    color: #2f322f;
 
-	font-family: $font;
-
-	// main scrollbar
+	// Main scrollbar
 	&::-webkit-scrollbar {
 		width: 7px;
 		background-color: inherit;
 	}
 	&::-webkit-scrollbar-thumb {
 		background-color: hsl($hue-signature, 21%, 71%);
-	}
-	&::-webkit-scrollbar-thumb:hover {
-		background-color: hsl($hue-signature, 21%, 50%);
+		&:hover {
+			background-color: hsl($hue-signature, 21%, 50%);
+		}
 	}
 }
 
 main {
 	min-height: 100vh;
-
-	width: 68%;
-	@media (max-width: $mobile-width) {
-		width: 91%;
-	}
-
 	margin: 0 auto;
-	margin-top: 41px;
-	margin-bottom: 81px;
-
-	font-family: $font2;
-	font-size: 17px;
-	@media (max-width: $mobile-width) {
-		font-size: $font-size-mobile;
-	}
-
-	color: hsl($hue-signature, 50%, 3%);
+	width: 68%;
+	@media (max-width: $mobile-width) {width: 91%;}
 
 	a {
 		color: inherit;
-	}
-	a:hover {
-		font-style: italic;
-	}
-
-	p {
-		line-height: 1.5;
+		&:hover {
+			color: hsl($hue-signature, 50%, 50%);
+		}
 	}
 
-	ul, ol {
-		line-height: 1.5;
-	}
-
-	img {
-		max-width: 100%;
-	}
+	// img {
+	// 	max-width: 100%;
+	// }
+}
 
-	pre, code {
-		background-color: hsl($hue-signature, 7%, 77%);
-		border-radius: 5px;
-		font-family: $font3;
-	}
-	pre {
-		padding: 11px 0;
-	}
-	code {
-		padding: 2px 5px;
-	}
+// I suspect these imports must be placed at the bottom,
+// or some SCSS styles might not be applied to them.
+// 
+//   					~ Nicholas @ July 12, 2023
+@import "header";
+@import "footer";
 
-	h1, h2 {
-		padding-top: 13px;
-	}
-}
+// Syntax highlighting
+@import "sass-code-highlight.scss";
```

### Comparing `nics-2.7.2/nics/main/_template/web/scripts/header.js` & `nics-2.8.1/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/compile/__init__.py` & `nics-2.8.1/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/compile/copying_template.py` & `nics-2.8.1/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/compile/update_404_and_favicon.py` & `nics-2.8.1/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/compile/update_docs_tree.py` & `nics-2.8.1/nics/main/compile/update_docs_tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
         ## <handling the index.md>
         if i == 'index.md':
             if base == '/':  # homepage
                 dst = os.path.join(D__PAGES, 'index.md')
                 text = (
                     '---\n'
-                    'permalink: /\n'
                     'layout: main\n'
                     'title: Home\n'
+                    'permalink: ""\n'
+                    'redirect_from:\n'
+                    '  - /\n'
                     '---\n\n'
                 )
                 with open(pth2, 'r') as f:
                     homepage = f.read()
                     if homepage.strip() == 'use-repo-readme':
                         printer('INFO: Using GitHub repo readme.')
                         repo_readme = requests.get(f'https://raw.githubusercontent.com/{gh_username}/{gh_repo}/main/README.md').text
@@ -43,17 +45,19 @@
                     else:
                         text += homepage
                 with open(dst, 'w') as f: f.write(text)
             else:
                 dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), 'index.md')
                 text = (
                     '---\n'
-                    f'permalink: {base}\n'
                     'layout: main\n'
                     f"title: {list(filter(lambda s:s!='', base.split('/')))[-1]}\n"
+                    f'permalink: {base[:-1]}\n'  # Trim the last '/'
+                    f'redirect_from:\n'
+                    f'  - {base}\n'
                     '---\n\n'
                 )
                 with open(pth2, 'r') as f: text += f.read()
                 with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated index.md from {repr(pth2)} to {repr(dst)}.')
             continue
         ## </handling the index.md>
@@ -73,17 +77,19 @@
                 printer(f'DEBUG: Dir created: {repr(dir)}.')
             ## do it again
             update_recursively(D__PAGES, lowercase_the_url, gh_username, gh_repo, pth2, base+url+'/')
         else:
             dst = os.path.join(D__PAGES, os.sep.join(filter(lambda s:s!='', base.split('/'))), f'{name}.md')
             text = (
                 '---\n'
-                f'permalink: {base}{url}/\n'
                 'layout: main\n'
                 f'title: {name}\n'
+                f'permalink: {base}{url}\n'
+                f'redirect_from:\n'
+                f'  - {base}{url}/\n'
                 '---\n\n'
             )
             with open(pth2, 'r') as f: text += f.read()
             with open(dst, 'w') as f: f.write(text)
             printer(f'DEBUG: Updated docs-tree file from {repr(pth2)} to {repr(dst)}.')
```

### Comparing `nics-2.7.2/nics/main/compile/update_header.py` & `nics-2.8.1/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/constants.py` & `nics-2.8.1/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/upgrade/__init__.py` & `nics-2.8.1/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/wizard/__init__.py` & `nics-2.8.1/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/wizard/settings_writer.py` & `nics-2.8.1/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics/main/wizard/workflow_writer.py` & `nics-2.8.1/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.7.2/nics.egg-info/SOURCES.txt` & `nics-2.8.1/nics.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 nics/main/_template/docs/tree/2 - Pages/logo200.png
 nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
 nics/main/_template/docs/tree/7 - FAQs/index.md
 nics/main/_template/web/_layouts/main.html
 nics/main/_template/web/_sass/footer.scss
 nics/main/_template/web/_sass/header.scss
 nics/main/_template/web/_sass/main.scss
+nics/main/_template/web/_sass/sass-code-highlight.scss
 nics/main/_template/web/scripts/header.js
 nics/main/compile/__init__.py
 nics/main/compile/copying_template.py
 nics/main/compile/inspect.py
 nics/main/compile/update_404_and_favicon.py
 nics/main/compile/update_docs_tree.py
 nics/main/compile/update_footer.py
```

### Comparing `nics-2.7.2/pyproject.toml` & `nics-2.8.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.7.2"
-description = "Automated markdown-based documentation tool"
+version = "2.8.1"
+description = "Automated markdown-based documentation page workflow"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "mykit==6.0.0",
+    "mykit==6.*",
     "requests>=2.31.0",
 ]
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "archive*",
```

### Comparing `nics-2.7.2/readme.md` & `nics-2.8.1/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 # Now I Can Sleep
 
-A minimalist, markdown-based tool for automating repository documentation creation.
+A minimalist, readable, easy-to-configure, and markdown-based automated documentation workflow for GitHub repositories.
+
+```txt
+🐈BEFORE🐈
+
+           ┌──────────>  Make changes  ────────────┐
+           |                                       v
+
+    Deploy docs-page                       Update docs-files
+
+           ^                                       │
+           └─────────  Rebuild docs-page  <────────┘
+
+
+
+🐾with NICS🐾
+
+           ┌──────────>  Make changes  ────────────┐
+           |                                       |
+           └─────────  Update docs-files  <────────┘
+```
 
 ![nics' banner](https://raw.githubusercontent.com/nvfp/now-i-can-sleep/master/assets/logo200.png)
 
 [![Rebuild docs](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml/badge.svg)](https://github.com/nvfp/now-i-can-sleep/actions/workflows/rebuild-docs.yml)
 [![pypi version](https://img.shields.io/pypi/v/nics?logo=pypi)](https://pypi.org/project/nics/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
```

