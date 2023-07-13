# Comparing `tmp/sphinx_code_tabs-0.5.3.tar.gz` & `tmp/sphinx_code_tabs-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_code_tabs-0.5.3.tar", last modified: Sun Nov 28 18:30:34 2021, max compression
+gzip compressed data, was "sphinx_code_tabs-0.5.5.tar", last modified: Thu Jul 13 10:53:21 2023, max compression
```

## Comparing `sphinx_code_tabs-0.5.3.tar` & `sphinx_code_tabs-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 18:30:34.259212 sphinx_code_tabs-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2021-11-28 18:30:34.259212 sphinx_code_tabs-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/UNLICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-11-28 18:30:34.259212 sphinx_code_tabs-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 18:30:34.259212 sphinx_code_tabs-0.5.3/sphinx_code_tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs/code-tabs.css
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs/code-tabs.js
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-11-28 18:30:24.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs/tabenv.sty
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-28 18:30:34.259212 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8037 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-28 18:30:34.000000 sphinx_code_tabs-0.5.3/sphinx_code_tabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:53:21.276258 sphinx_code_tabs-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-13 10:53:21.276258 sphinx_code_tabs-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/UNLICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-13 10:53:21.276258 sphinx_code_tabs-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:53:21.276258 sphinx_code_tabs-0.5.5/sphinx_code_tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs/code-tabs.css
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs/code-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-13 10:52:54.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs/tabenv.sty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:53:21.276258 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 10:53:21.000000 sphinx_code_tabs-0.5.5/sphinx_code_tabs.egg-info/top_level.txt
```

### Comparing `sphinx_code_tabs-0.5.3/README.rst` & `sphinx_code_tabs-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_code_tabs-0.5.3/UNLICENSE` & `sphinx_code_tabs-0.5.5/UNLICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_code_tabs-0.5.3/setup.cfg` & `sphinx_code_tabs-0.5.5/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 url = https://github.com/coldfix/sphinx-code-tabs
 download_url = https://pypi.org/project/sphinx_code_tabs
 long_description = file: README.rst, CHANGES.rst
 author = Thomas Gläßle
 author_email = thomas@coldfix.de
 license = Unlicense
 license_file = UNLICENSE
+project_urls = 
+	Source Code = https://github.com/coldfix/sphinx-code-tabs
+	Bug Tracker = https://github.com/coldfix/sphinx-code-tabs/issues
+	Documentation = https://sphinx-code-tabs.readthedocs.io
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Plugins
 	Intended Audience :: Developers
 	License :: OSI Approved :: The Unlicense (Unlicense)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
```

### Comparing `sphinx_code_tabs-0.5.3/sphinx_code_tabs/__init__.py` & `sphinx_code_tabs-0.5.5/sphinx_code_tabs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.3'
+__version__ = '0.5.5'
 
 from docutils.parsers.rst import directives
 from docutils import nodes
 from sphinx.directives.code import CodeBlock
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.fileutil import copy_asset_file
 
@@ -222,7 +222,12 @@
         html=(visit_tab_html, depart_tab_html),
         latex=(visit_tab_latex, depart_tab_latex))
     app.add_directive("tabs", TabsDirective)
     app.add_directive("tab", TabDirective)
     app.add_directive("code-tabs", TabsDirective)
     app.add_directive("code-tab", CodeTabDirective)
     app.connect("builder-inited", add_assets)
+
+    return {
+        "version": __version__,
+        "parallel_read_safe": True,
+    }
```

### Comparing `sphinx_code_tabs-0.5.3/sphinx_code_tabs/code-tabs.css` & `sphinx_code_tabs-0.5.5/sphinx_code_tabs/code-tabs.css`

 * *Files identical despite different names*

### Comparing `sphinx_code_tabs-0.5.3/sphinx_code_tabs/code-tabs.js` & `sphinx_code_tabs-0.5.5/sphinx_code_tabs/code-tabs.js`

 * *Files identical despite different names*

### Comparing `sphinx_code_tabs-0.5.3/sphinx_code_tabs/tabenv.sty` & `sphinx_code_tabs-0.5.5/sphinx_code_tabs/tabenv.sty`

 * *Files identical despite different names*

