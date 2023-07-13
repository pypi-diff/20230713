# Comparing `tmp/st_pandas_text_editor-0.0.5.tar.gz` & `tmp/st_pandas_text_editor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pandas_text_editor-0.0.5.tar", last modified: Thu Jul 13 09:14:58 2023, max compression
+gzip compressed data, was "st_pandas_text_editor-0.0.6.tar", last modified: Thu Jul 13 09:20:22 2023, max compression
```

## Comparing `st_pandas_text_editor-0.0.5.tar` & `st_pandas_text_editor-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.896757 st_pandas_text_editor-0.0.5/
--rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      287 2023-07-13 09:14:58.895346 st_pandas_text_editor-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 09:14:58.896757 st_pandas_text_editor-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-07-13 09:14:44.000000 st_pandas_text_editor-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.583600 st_pandas_text_editor-0.0.5/st_pandas_text_editor/
--rw-rw-rw-   0        0        0     5235 2023-07-13 09:13:36.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.565937 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.635777 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/
--rw-rw-rw-   0        0        0     1078 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2232 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.567193 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.659233 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/
--rw-rw-rw-   0        0        0    17207 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
--rw-rw-rw-   0        0        0    30841 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
--rw-rw-rw-   0        0        0      348 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
--rw-rw-rw-   0        0        0      788 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.894293 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/
--rw-rw-rw-   0        0        0  1051761 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js
--rw-rw-rw-   0        0        0     2322 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  3774469 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map
--rw-rw-rw-   0        0        0     5379 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js
--rw-rw-rw-   0        0        0    15704 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.603430 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/
--rw-rw-rw-   0        0        0      287 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.347356 st_pandas_text_editor-0.0.6/
+-rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      287 2023-07-13 09:20:22.347356 st_pandas_text_editor-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:20:22.348357 st_pandas_text_editor-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-07-13 09:19:41.000000 st_pandas_text_editor-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.100684 st_pandas_text_editor-0.0.6/st_pandas_text_editor/
+-rw-rw-rw-   0        0        0     5234 2023-07-13 09:19:59.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.088673 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.124647 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/
+-rw-rw-rw-   0        0        0     1078 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2232 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.091287 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.140179 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/
+-rw-rw-rw-   0        0        0    17207 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
+-rw-rw-rw-   0        0        0    30841 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
+-rw-rw-rw-   0        0        0      348 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
+-rw-rw-rw-   0        0        0      788 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.346347 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/
+-rw-rw-rw-   0        0        0  1051761 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js
+-rw-rw-rw-   0        0        0     2322 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  3774469 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map
+-rw-rw-rw-   0        0        0     5379 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js
+-rw-rw-rw-   0        0        0    15704 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-13 09:20:16.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-13 09:20:22.113676 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-13 09:20:21.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-07-13 09:20:21.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:20:21.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 09:20:21.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-13 09:20:21.000000 st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/top_level.txt
```

### Comparing `st_pandas_text_editor-0.0.5/LICENSE` & `st_pandas_text_editor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/README.md` & `st_pandas_text_editor-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/setup.py` & `st_pandas_text_editor-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_pandas_text_editor",
-    version="0.0.5",
+    version="0.0.6",
     author="Elias",
     author_email="eli.mue@gmx.de",
     description="Rich Text Editor with customizable Dropdown Options for Streamlit",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/__init__.py` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/asset-manifest.json` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/bootstrap.min.css` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/index.html` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/SOURCES.txt` & `st_pandas_text_editor-0.0.6/st_pandas_text_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

