# Comparing `tmp/nics-2.8.3.tar.gz` & `tmp/nics-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-z50dyfl9/nics-2.8.3.tar", last modified: Thu Jul 13 18:24:08 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-j2pr5lfj/nics-2.8.4.tar", last modified: Thu Jul 13 18:36:06 2023, max compression
```

## Comparing `nics-2.8.3.tar` & `nics-2.8.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 18:24:00.000000 nics-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 18:24:00.000000 nics-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:24:08.000000 nics-2.8.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 18:24:00.000000 nics-2.8.3/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/404.md
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/docs/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/2 - Pages/baz.md
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/2 - Pages/logo200.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/docs/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/_sass/main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/_sass/sass-code-highlight.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-13 18:24:00.000000 nics-2.8.3/nics/main/wizard/workflow_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 18:24:08.000000 nics-2.8.3/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 18:24:01.000000 nics-2.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 18:24:00.000000 nics-2.8.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 18:24:08.000000 nics-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 18:24:00.000000 nics-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 18:35:58.000000 nics-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 18:35:58.000000 nics-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:36:06.000000 nics-2.8.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 18:35:58.000000 nics-2.8.4/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/baz.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/logo200.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/_sass/sass-code-highlight.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-13 18:35:58.000000 nics-2.8.4/nics/main/wizard/workflow_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 18:36:06.000000 nics-2.8.4/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 18:35:58.000000 nics-2.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 18:35:58.000000 nics-2.8.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 18:36:06.000000 nics-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 18:35:58.000000 nics-2.8.4/setup.py
```

### Comparing `nics-2.8.3/LICENSE` & `nics-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/PKG-INFO` & `nics-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.8.3
+Version: 2.8.4
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.8.3/nics/main/__init__.py` & `nics-2.8.4/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/docs/favicon.png` & `nics-2.8.4/nics/main/_template/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/docs/tree/2 - Pages/logo200.png` & `nics-2.8.4/nics/main/_template/docs/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/web/_sass/header.scss` & `nics-2.8.4/nics/main/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/web/_sass/main.scss` & `nics-2.8.4/nics/main/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/web/_sass/sass-code-highlight.scss` & `nics-2.8.4/nics/main/_template/web/_sass/sass-code-highlight.scss`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/_template/web/scripts/header.js` & `nics-2.8.4/nics/main/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/compile/__init__.py` & `nics-2.8.4/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/compile/update_404_and_favicon.py` & `nics-2.8.4/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/compile/update_docs_tree.py` & `nics-2.8.4/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/compile/update_header.py` & `nics-2.8.4/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/compile/update_jekyll_config.py` & `nics-2.8.4/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/constants.py` & `nics-2.8.4/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/upgrade/__init__.py` & `nics-2.8.4/nics/main/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/wizard/__init__.py` & `nics-2.8.4/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/wizard/settings_writer.py` & `nics-2.8.4/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics/main/wizard/workflow_writer.py` & `nics-2.8.4/nics/main/wizard/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/nics.egg-info/PKG-INFO` & `nics-2.8.4/nics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 2.8.3
+Version: 2.8.4
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-2.8.3/nics.egg-info/SOURCES.txt` & `nics-2.8.4/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-2.8.3/pyproject.toml` & `nics-2.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "2.8.3"
+version = "2.8.4"
 description = "Automated markdown-based documentation page workflow"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

### Comparing `nics-2.8.3/readme.md` & `nics-2.8.4/readme.md`

 * *Files identical despite different names*

