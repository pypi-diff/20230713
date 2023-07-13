# Comparing `tmp/st_pandas_text_editor-0.0.4.tar.gz` & `tmp/st_pandas_text_editor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pandas_text_editor-0.0.4.tar", last modified: Wed Jul 12 15:48:32 2023, max compression
+gzip compressed data, was "st_pandas_text_editor-0.0.5.tar", last modified: Thu Jul 13 09:14:58 2023, max compression
```

## Comparing `st_pandas_text_editor-0.0.4.tar` & `st_pandas_text_editor-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:32.129812 st_pandas_text_editor-0.0.4/
--rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      287 2023-07-12 15:48:32.129812 st_pandas_text_editor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 15:48:32.131106 st_pandas_text_editor-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-07-12 15:46:13.000000 st_pandas_text_editor-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.888527 st_pandas_text_editor-0.0.4/st_pandas_text_editor/
--rw-rw-rw-   0        0        0     5120 2023-07-12 15:42:32.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.879169 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.906899 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/
--rw-rw-rw-   0        0        0     1078 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2232 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.880612 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.924185 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/
--rw-rw-rw-   0        0        0    17207 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
--rw-rw-rw-   0        0        0    30841 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
--rw-rw-rw-   0        0        0      348 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
--rw-rw-rw-   0        0        0      788 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:32.128633 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/
--rw-rw-rw-   0        0        0  1051761 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js
--rw-rw-rw-   0        0        0     2322 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  3774473 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map
--rw-rw-rw-   0        0        0     5292 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js
--rw-rw-rw-   0        0        0    15354 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-12 15:48:25.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-12 15:48:31.895428 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/
--rw-rw-rw-   0        0        0      287 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-12 15:48:31.000000 st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.896757 st_pandas_text_editor-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2023-07-05 07:54:54.000000 st_pandas_text_editor-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-05 08:05:30.000000 st_pandas_text_editor-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      287 2023-07-13 09:14:58.895346 st_pandas_text_editor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6321 2023-07-05 07:56:06.000000 st_pandas_text_editor-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:14:58.896757 st_pandas_text_editor-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-07-13 09:14:44.000000 st_pandas_text_editor-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.583600 st_pandas_text_editor-0.0.5/st_pandas_text_editor/
+-rw-rw-rw-   0        0        0     5235 2023-07-13 09:13:36.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.565937 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.635777 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/
+-rw-rw-rw-   0        0        0     1078 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-05 14:47:49.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2232 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.567193 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.659233 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/
+-rw-rw-rw-   0        0        0    17207 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
+-rw-rw-rw-   0        0        0    30841 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
+-rw-rw-rw-   0        0        0      348 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
+-rw-rw-rw-   0        0        0      788 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.894293 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/
+-rw-rw-rw-   0        0        0  1051761 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js
+-rw-rw-rw-   0        0        0     2322 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  3774469 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map
+-rw-rw-rw-   0        0        0     5379 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js
+-rw-rw-rw-   0        0        0    15704 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-13 09:14:47.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-13 09:14:58.603430 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-13 09:14:58.000000 st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/top_level.txt
```

### Comparing `st_pandas_text_editor-0.0.4/LICENSE` & `st_pandas_text_editor-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/README.md` & `st_pandas_text_editor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/setup.py` & `st_pandas_text_editor-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_pandas_text_editor",
-    version="0.0.4",
+    version="0.0.5",
     author="Elias",
     author_email="eli.mue@gmx.de",
     description="Rich Text Editor with customizable Dropdown Options for Streamlit",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/__init__.py` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = True
+_RELEASE = False
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
@@ -43,17 +43,18 @@
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 def st_pandas_text_editor(
     columns,
-    key=None,
+    value,
+    key,
+    placeholder,
     agg=["mean", "sum", "var", "std", "nunique", "unique"],
-    placeholder="",
 ):
     """Create a new instance of "st_pandas_text_editor".
 
     Parameters
     ----------
     name: str
         The name of the thing we're saying hello to. The component will display
@@ -74,15 +75,20 @@
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
     component_value = _component_func(
-        columns=columns, key=key, default=0, agg=agg, placeholder=placeholder
+        columns=columns,
+        key=key,
+        default=0,
+        agg=agg,
+        placeholder=placeholder,
+        value=value,
     )
 
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
 
 
@@ -108,15 +114,18 @@
     #
     # We use the special "key" argument to assign a fixed identity to this
     # component instance. By default, when a component's arguments change,
     # it is considered a new instance and will be re-mounted on the frontend
     # and lose its current state. In this case, we want to vary the component's
     # "name" argument without having it get recreated.
     response = st_pandas_text_editor(
-        columns=df.columns.tolist(), key="foo", placeholder="This is ...\n a story"
+        columns=df.columns.tolist(),
+        key="foo",
+        placeholder="This is ...\n a story",
+        value="Initial Value",
     )
     if response:
         print(response)
         st.write(response)
         # use eval to dynamically evaluate the string (unsafe --> minimze risks)
         st.write(eval(f'f"""{response[1]}"""'))
         st.write(response[2])
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/asset-manifest.json` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/asset-manifest.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7404761904761905%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.817968fe.chunk.js'), (4, "*

 * *                  "'static/js/main.7e37a4e5.chunk.js')], delete: [4, 2]}",*

 * * "'files'": "{'main.js': './static/js/main.7e37a4e5.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.7e37a4e5.chunk.js.map', 'static/js/2.817968fe.chunk.js': "*

 * *            "'./static/js/2.817968fe.chunk.js', 'static/js/2.817968fe.chunk.js.map': "*

 * *            "'./static/js/2.817968fe.chunk.js.map', 'static/js/2.817968fe.chunk.js.LICENSE.txt': "*

 * *         […]*

```diff
@@ -1,23 +1,23 @@
 {
     "entrypoints": [
         "static/js/runtime-main.624f085e.js",
         "static/css/2.9b7094a5.chunk.css",
-        "static/js/2.ecfcc7a3.chunk.js",
+        "static/js/2.817968fe.chunk.js",
         "static/css/main.c21eaae6.chunk.css",
-        "static/js/main.baa131a3.chunk.js"
+        "static/js/main.7e37a4e5.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.c21eaae6.chunk.css",
-        "main.js": "./static/js/main.baa131a3.chunk.js",
-        "main.js.map": "./static/js/main.baa131a3.chunk.js.map",
+        "main.js": "./static/js/main.7e37a4e5.chunk.js",
+        "main.js.map": "./static/js/main.7e37a4e5.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.624f085e.js",
         "runtime-main.js.map": "./static/js/runtime-main.624f085e.js.map",
         "static/css/2.9b7094a5.chunk.css": "./static/css/2.9b7094a5.chunk.css",
         "static/css/2.9b7094a5.chunk.css.map": "./static/css/2.9b7094a5.chunk.css.map",
         "static/css/main.c21eaae6.chunk.css.map": "./static/css/main.c21eaae6.chunk.css.map",
-        "static/js/2.ecfcc7a3.chunk.js": "./static/js/2.ecfcc7a3.chunk.js",
-        "static/js/2.ecfcc7a3.chunk.js.LICENSE.txt": "./static/js/2.ecfcc7a3.chunk.js.LICENSE.txt",
-        "static/js/2.ecfcc7a3.chunk.js.map": "./static/js/2.ecfcc7a3.chunk.js.map"
+        "static/js/2.817968fe.chunk.js": "./static/js/2.817968fe.chunk.js",
+        "static/js/2.817968fe.chunk.js.LICENSE.txt": "./static/js/2.817968fe.chunk.js.LICENSE.txt",
+        "static/js/2.817968fe.chunk.js.map": "./static/js/2.817968fe.chunk.js.map"
     }
 }
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/bootstrap.min.css` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/index.html` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.9b7094a5.chunk.css" rel="stylesheet"><link href="./static/css/main.c21eaae6.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.ecfcc7a3.chunk.js"></script><script src="./static/js/main.baa131a3.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.9b7094a5.chunk.css" rel="stylesheet"><link href="./static/css/main.c21eaae6.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.817968fe.chunk.js"></script><script src="./static/js/main.7e37a4e5.chunk.js"></script></body></html>
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.ecfcc7a3.chunk.js.LICENSE.txt */
+/*! For license information please see 2.817968fe.chunk.js.LICENSE.txt */
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [2],
     [function(t, e, n) {
         "use strict";
 
         function r(t, e) {
             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
@@ -5804,14 +5804,66 @@
             o = Math.pow(2, 24);
         t.exports = function() {
             for (var t; void 0 === t || r.hasOwnProperty(t) || !isNaN(+t);) t = Math.floor(Math.random() * o).toString(32);
             return r[t] = !0, t
         }
     }, function(t, e, n) {
         "use strict";
+        var r = n(118),
+            o = n(38),
+            i = n(19),
+            a = n(134),
+            u = n(29),
+            c = n(59),
+            s = n(61),
+            l = n(78),
+            f = n(135),
+            p = n(94),
+            d = n(47),
+            h = n(16),
+            y = n(76),
+            v = n(13),
+            g = n(67),
+            b = n(202),
+            m = n(105),
+            w = n(48),
+            _ = n(203),
+            k = n(206),
+            O = n(23),
+            S = n(106),
+            j = n(212),
+            x = {
+                Editor: f,
+                EditorBlock: p,
+                EditorState: v,
+                CompositeDecorator: a,
+                Entity: d,
+                EntityInstance: y,
+                BlockMapBuilder: o,
+                CharacterMetadata: i,
+                ContentBlock: u,
+                ContentState: c,
+                RawDraftContentState: b,
+                SelectionState: w,
+                AtomicBlockUtils: r,
+                KeyBindingUtil: g,
+                Modifier: h,
+                RichUtils: m,
+                DefaultDraftBlockRenderMap: s,
+                DefaultDraftInlineStyle: l,
+                convertFromHTML: n(103),
+                convertFromRaw: k,
+                convertToRaw: _,
+                genKey: O,
+                getDefaultKeyBinding: S,
+                getVisibleSelectionRect: j
+            };
+        t.exports = x
+    }, function(t, e, n) {
+        "use strict";
         var r = Object.getOwnPropertySymbols,
             o = Object.prototype.hasOwnProperty,
             i = Object.prototype.propertyIsEnumerable;
         t.exports = function() {
             try {
                 if (!Object.assign) return !1;
                 var t = new String("abc");
@@ -5875,66 +5927,14 @@
     }, function(t, e, n) {
         "use strict";
         t.exports = function(t) {
             return !("undefined" === typeof window || !window.__DRAFT_GKX) && !!window.__DRAFT_GKX[t]
         }
     }, function(t, e, n) {
         "use strict";
-        var r = n(118),
-            o = n(38),
-            i = n(19),
-            a = n(134),
-            u = n(29),
-            c = n(59),
-            s = n(61),
-            l = n(78),
-            f = n(135),
-            p = n(94),
-            d = n(47),
-            h = n(16),
-            y = n(76),
-            v = n(13),
-            g = n(67),
-            b = n(202),
-            m = n(105),
-            w = n(48),
-            _ = n(203),
-            k = n(206),
-            O = n(23),
-            S = n(106),
-            j = n(212),
-            x = {
-                Editor: f,
-                EditorBlock: p,
-                EditorState: v,
-                CompositeDecorator: a,
-                Entity: d,
-                EntityInstance: y,
-                BlockMapBuilder: o,
-                CharacterMetadata: i,
-                ContentBlock: u,
-                ContentState: c,
-                RawDraftContentState: b,
-                SelectionState: w,
-                AtomicBlockUtils: r,
-                KeyBindingUtil: g,
-                Modifier: h,
-                RichUtils: m,
-                DefaultDraftBlockRenderMap: s,
-                DefaultDraftInlineStyle: l,
-                convertFromHTML: n(103),
-                convertFromRaw: k,
-                convertToRaw: _,
-                genKey: O,
-                getDefaultKeyBinding: S,
-                getVisibleSelectionRect: j
-            };
-        t.exports = x
-    }, function(t, e, n) {
-        "use strict";
         var r = n(19),
             o = n(39),
             i = n(11),
             a = i.List,
             u = i.Map,
             c = i.OrderedSet,
             s = i.Record,
@@ -6076,15 +6076,15 @@
         };
         t.exports = f
     }, function(t, e, n) {
         "use strict";
         n.d(e, "a", (function() {
             return i
         }));
-        var r = n(26),
+        var r = n(27),
             o = n(34);
 
         function i(t, e) {
             if (e && ("object" === Object(r.a)(e) || "function" === typeof e)) return e;
             if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
             return Object(o.a)(t)
         }
@@ -6172,15 +6172,15 @@
         "use strict";
         t.exports = function(t) {
             return !(!t || !t.ownerDocument) && (t.ownerDocument.defaultView ? t instanceof t.ownerDocument.defaultView.HTMLElement : t instanceof HTMLElement)
         }
     }, function(t, e, n) {
         "use strict";
         var r = n(16),
-            o = n(27)("draft_tree_data_support");
+            o = n(28)("draft_tree_data_support");
         t.exports = function(t, e, n) {
             var i = t.getSelection(),
                 a = t.getCurrentContent(),
                 u = i,
                 c = i.getAnchorKey(),
                 s = i.getFocusKey(),
                 l = a.getBlockForKey(c);
@@ -6695,15 +6695,15 @@
                     }
                     a(void 0)
                 }))
             }
         }
         var A = n(0),
             L = n(1),
-            N = n(26);
+            N = n(27);
 
         function z() {
             z = function() {
                 return t
             };
             var t = {},
                 e = Object.prototype,
@@ -22758,15 +22758,15 @@
             e.a = i || o ? r.useLayoutEffect : r.useEffect
         }).call(this, n(40))
     }, function(t, e, n) {
         "use strict";
         n.d(e, "a", (function() {
             return o
         }));
-        var r = n(26);
+        var r = n(27);
 
         function o(t) {
             var e = function(t, e) {
                 if ("object" !== Object(r.a)(t) || null === t) return t;
                 var n = t[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var o = n.call(t, e || "default");
@@ -22805,15 +22805,15 @@
             a = n(19),
             u = n(29),
             c = n(20),
             s = n(47),
             l = n(48),
             f = n(23),
             p = n(75),
-            d = n(27),
+            d = n(28),
             h = n(11),
             y = n(77),
             v = h.List,
             g = h.Record,
             b = h.Repeat,
             m = h.Map,
             w = h.OrderedMap,
@@ -23471,15 +23471,15 @@
             }, p = s(e, n, o)) : (p = s(e, n, o), d = s(e, a, u), n === a && o === u && (h = !!n.firstChild && "BR" !== n.firstChild.nodeName)), {
                 selectionState: i(t, p.key, p.offset, d.key, d.offset),
                 needsRecovery: h
             }
         }
     }, function(t, e, n) {
         "use strict";
-        var r = n(25),
+        var r = n(26),
             o = n(17);
         t.exports = function(t, e, n, i, a) {
             var u = o(t.getSelection());
             if (!e || !i) return u;
             var c = r.decode(e),
                 s = c.blockKey,
                 l = t.getBlockTree(s),
@@ -23517,15 +23517,15 @@
         t.exports = {
             notEmptyKey: function(t) {
                 return null != t && "" != t
             }
         }
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
         var o = n(149),
             i = n(4),
             a = n(12),
             u = n(89),
             c = n(150).setDraftEditorSelection,
             s = function(t) {
                 var e, n;
@@ -23653,27 +23653,27 @@
             return {
                 width: r(),
                 height: o()
             }
         }, t.exports = i
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
 
         function o() {
             return o = r || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                 }
                 return t
             }, o.apply(this, arguments)
         }
         var i = n(88),
-            a = n(25),
+            a = n(26),
             u = n(4),
             c = n(64),
             s = n(53),
             l = n(60),
             f = n(49),
             p = n(30),
             d = n(92),
@@ -24008,15 +24008,15 @@
             c = n(20),
             s = n(61),
             l = n(47),
             f = n(195),
             p = n(30),
             d = n(23),
             h = n(104),
-            y = n(27),
+            y = n(28),
             v = n(11),
             g = v.List,
             b = v.Map,
             m = v.OrderedSet,
             w = n(196),
             _ = n(89),
             k = n(41),
@@ -32971,15 +32971,15 @@
                     i: t,
                     l: !1,
                     exports: {}
                 };
                 return o[t].call(e.exports, e, e.exports, r), e.l = !0, e.exports
             }
             var o, i
-        }(n(4), n(28), n(214))
+        }(n(4), n(24), n(214))
     }, function(t, e, n) {
         t.exports = function() {
             "use strict";
 
             function t(t, e) {
                 if (t)
                     for (var n in t)({}).hasOwnProperty.call(t, n) && e(n, t[n])
@@ -33261,15 +33261,15 @@
                 }
                 return o.join("")
             }
             return j
         }()
     }, , function(t, e, n) {
         "use strict";
-        var r = n(24),
+        var r = n(25),
             o = "function" === typeof Symbol && Symbol.for,
             i = o ? Symbol.for("react.element") : 60103,
             a = o ? Symbol.for("react.portal") : 60106,
             u = o ? Symbol.for("react.fragment") : 60107,
             c = o ? Symbol.for("react.strict_mode") : 60108,
             s = o ? Symbol.for("react.profiler") : 60114,
             l = o ? Symbol.for("react.provider") : 60109,
@@ -33565,15 +33565,15 @@
             return F().useRef(t)
         }, e.useState = function(t) {
             return F().useState(t)
         }, e.version = "16.14.0"
     }, function(t, e, n) {
         "use strict";
         var r = n(4),
-            o = n(24),
+            o = n(25),
             i = n(114);
 
         function a(t) {
             for (var e = "https://reactjs.org/docs/error-decoder.html?invariant=" + t, n = 1; n < arguments.length; n++) e += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified React error #" + t + "; visit " + e + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
         }
         if (!r) throw Error(a(227));
@@ -39184,15 +39184,15 @@
         var i = n(38),
             a = n(19),
             u = n(29),
             c = n(20),
             s = n(16),
             l = n(13),
             f = n(23),
-            p = n(27),
+            p = n(28),
             d = n(11),
             h = n(133),
             y = p("draft_tree_data_support"),
             v = y ? c : u,
             g = d.List,
             b = d.Repeat,
             m = {
@@ -40178,15 +40178,15 @@
                     return this._decorators[e].props
                 }, t
             }();
         t.exports = o
     }, function(t, e, n) {
         "use strict";
         (function(e) {
-            var r = n(24);
+            var r = n(25);
 
             function o() {
                 return o = r || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
                         for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                     }
@@ -40238,15 +40238,15 @@
                 w = n(64),
                 _ = n(53),
                 k = n(18),
                 O = n(30),
                 S = n(23),
                 j = n(106),
                 x = n(54),
-                E = n(27),
+                E = n(28),
                 M = n(12),
                 T = n(41),
                 I = n(17),
                 C = k.isBrowser("IE"),
                 D = !C,
                 A = {
                     edit: h,
@@ -40470,15 +40470,15 @@
                 stripPastedStyles: !1
             }), t.exports = z
         }).call(this, n(40))
     }, function(t, e, n) {
         "use strict";
         var r = n(137),
             o = n(16),
-            i = n(25),
+            i = n(26),
             a = n(13),
             u = n(52),
             c = n(18),
             s = n(81),
             l = n(83),
             f = n(84),
             p = n(62),
@@ -41501,31 +41501,31 @@
             var e = {};
             return function(n) {
                 return e.hasOwnProperty(n) || (e[n] = t.call(this, n)), e[n]
             }
         }
     }, function(t, e, n) {
         "use strict";
-        var r = n(27)("draft_tree_data_support");
+        var r = n(28)("draft_tree_data_support");
         t.exports = n(r ? 145 : 159)
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
 
         function o() {
             return o = r || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                 }
                 return t
             }, o.apply(this, arguments)
         }
         var i = n(146),
-            a = n(25),
+            a = n(26),
             u = n(4),
             c = n(17),
             s = function(t) {
                 var e, n;
 
                 function r() {
                     return t.apply(this, arguments) || this
@@ -41595,15 +41595,15 @@
                         "data-contents": "true"
                     }, j)
                 }, r
             }(u.Component);
         t.exports = s
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
 
         function o() {
             return o = r || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                 }
@@ -41629,15 +41629,15 @@
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : t[e] = n, t
         }
         var u = n(147),
-            c = n(25),
+            c = n(26),
             s = n(4),
             l = n(64),
             f = n(53),
             p = n(92),
             d = n(54),
             h = n(93),
             y = n(11),
@@ -41808,15 +41808,15 @@
                 }, r
             }(s.Component);
         t.exports = k
     }, function(t, e, n) {
         "use strict";
         var r = n(148),
             o = n(88),
-            i = n(25),
+            i = n(26),
             a = n(11),
             u = n(4),
             c = n(30),
             s = (a.List, function(t) {
                 var e, n;
 
                 function a() {
@@ -41880,26 +41880,26 @@
                         })
                     }, m)
                 }, a
             }(u.Component));
         t.exports = s
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
 
         function o() {
             return o = r || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                 }
                 return t
             }, o.apply(this, arguments)
         }
-        var i = n(25),
+        var i = n(26),
             a = n(4),
             u = n(60),
             c = n(49),
             s = function(t) {
                 var e, n;
 
                 function r() {
@@ -42211,15 +42211,15 @@
             } : {
                 x: t.scrollLeft,
                 y: t.scrollTop
             }
         }
     }, function(t, e, n) {
         "use strict";
-        var r = n(24);
+        var r = n(25);
 
         function o() {
             return o = r || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = arguments[e];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (t[r] = n[r])
                 }
@@ -42245,15 +42245,15 @@
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : t[e] = n, t
         }
         var u = n(94),
-            c = n(25),
+            c = n(26),
             s = n(4),
             l = n(30),
             f = n(160),
             p = n(17),
             d = function(t, e, n, r) {
                 return l({
                     "public/DraftStyleDefault/unorderedListItem": "unordered-list-item" === t,
@@ -42870,15 +42870,15 @@
                 var a = i.set("hasFocus", !0);
                 t.props.onFocus && t.props.onFocus(e), o.isBrowser("Chrome < 60.0.3081.0") ? t.update(r.forceSelection(n, a)) : t.update(r.acceptSelection(n, a))
             }
         }
     }, function(t, e, n) {
         "use strict";
         var r = n(16),
-            o = n(25),
+            o = n(26),
             i = n(13),
             a = n(18),
             u = n(87).notEmptyKey,
             c = n(50),
             s = n(99),
             l = n(17),
             f = a.isEngine("Gecko");
@@ -43394,15 +43394,15 @@
             }) : t[e] = n, t
         }
         var o = n(29),
             i = n(20),
             a = n(103),
             u = n(23),
             c = n(104),
-            s = n(27),
+            s = n(28),
             l = n(11),
             f = n(77),
             p = l.List,
             d = l.Repeat,
             h = s("draft_tree_data_support"),
             y = h ? i : o,
             v = {
@@ -43707,15 +43707,15 @@
             c = n(47),
             s = n(207),
             l = (n(208), n(48)),
             f = n(209),
             p = n(210),
             d = n(211),
             h = n(23),
-            y = n(27),
+            y = n(28),
             v = n(11),
             g = n(12),
             b = y("draft_tree_data_support"),
             m = v.List,
             w = v.Map,
             _ = v.OrderedMap,
             k = function(t, e) {
@@ -46632,8 +46632,8 @@
                 props: i,
                 _owner: a.current
             }
         }
         e.jsx = s, e.jsxs = s
     }]
 ]);
-//# sourceMappingURL=2.ecfcc7a3.chunk.js.map
+//# sourceMappingURL=2.817968fe.chunk.js.map
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8561009282877956%*

 * *Differences: {"'file'": "'static/js/2.817968fe.chunk.js'",*

 * * "'mappings'": "';0IAAe,SAASA,EAAgBC,EAAUC,GAChD,KAAMD,aAAoBC,GACxB,MAAM,IAAIC,UAAU,oCAExB,CAJA,iC,+BCAA,8CACA,SAASC,EAAkBC,EAAQC,GACjC,IAAK,IAAIC,EAAI,EAAGA,EAAID,EAAME,OAAQD,IAAK,CACrC,IAAIE,EAAaH,EAAMC,GACvBE,EAAWC,WAAaD,EAAWC,aAAc,EACjDD,EAAWE,cAAe,EACtB,UAAWF,IAAYA,EAAWG,UAAW,GACjDC,OAAOC,eAAeT,EAAQ,YAAcI,EAAWM,KAAMN,EAC/D,CACF,CACe,SAASO,EAAad,EAAae,EAAYC,GAM5D,OALID,GAAYb,EAAkBF,EAAYiB,UAAWF,GACrDC,GAAad,EAAkBF,EAAagB,GAChDL,OAAOC,eAAeZ,EAAa,YAAa,CAC9CU,U […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.ecfcc7a3.chunk.js",
+    "file": "static/js/2.817968fe.chunk.js",
     "names": [
         "_classCallCheck",
         "instance",
         "Constructor",
         "TypeError",
         "_defineProperties",
         "target",
@@ -1783,33 +1783,14 @@
         "ItemText",
         "Divider",
         "Header",
         "seenKeys",
         "MULTIPLIER",
         "pow",
         "isNaN",
-        "propIsEnumerable",
-        "test1",
-        "getOwnPropertyNames",
-        "test2",
-        "fromCharCode",
-        "test3",
-        "letter",
-        "shouldUseNative",
-        "KEY_DELIMITER",
-        "DraftOffsetKey",
-        "encode",
-        "decoratorKey",
-        "leafKey",
-        "decode",
-        "offsetKey",
-        "_offsetKey$split$reve",
-        "parseInt",
-        "_typeof",
-        "__DRAFT_GKX",
         "AtomicBlockUtils",
         "BlockMapBuilder",
         "CompositeDraftDecorator",
         "ContentBlock",
         "DefaultDraftBlockRenderMap",
         "DefaultDraftInlineStyle",
         "DraftEditor",
@@ -1832,14 +1813,33 @@
         "EntityInstance",
         "Modifier",
         "RichUtils",
         "convertFromHTML",
         "convertFromRaw",
         "convertToRaw",
         "genKey",
+        "propIsEnumerable",
+        "test1",
+        "getOwnPropertyNames",
+        "test2",
+        "fromCharCode",
+        "test3",
+        "letter",
+        "shouldUseNative",
+        "KEY_DELIMITER",
+        "DraftOffsetKey",
+        "encode",
+        "decoratorKey",
+        "leafKey",
+        "decode",
+        "offsetKey",
+        "_offsetKey$split$reve",
+        "parseInt",
+        "_typeof",
+        "__DRAFT_GKX",
         "ContentBlockRecord",
         "_ContentBlockRecord",
         "Node",
         "ELEMENT_NODE",
         "SURROGATE_HIGH_START",
         "SURROGATE_LOW_END",
         "SURROGATE_UNITS_REGEX",
@@ -7028,19 +7028,19 @@
         "../node_modules/react-bootstrap/esm/DropdownMenu.js",
         "../node_modules/react-bootstrap/esm/Button.js",
         "../node_modules/react-bootstrap/esm/DropdownToggle.js",
         "../node_modules/dom-helpers/esm/camelize.js",
         "../node_modules/react-bootstrap/esm/createWithBsPrefix.js",
         "../node_modules/react-bootstrap/esm/Dropdown.js",
         "../node_modules/draft-js/lib/generateRandomKey.js",
+        "../node_modules/draft-js/lib/Draft.js",
         "../node_modules/object-assign/index.js",
         "../node_modules/draft-js/lib/DraftOffsetKey.js",
         "../node_modules/@babel/runtime/helpers/esm/typeof.js",
         "../node_modules/draft-js/lib/gkx.js",
-        "../node_modules/draft-js/lib/Draft.js",
         "../node_modules/draft-js/lib/ContentBlock.js",
         "../node_modules/fbjs/lib/cx.js",
         "../node_modules/draft-js/lib/isElement.js",
         "../node_modules/fbjs/lib/UnicodeUtils.js",
         "../node_modules/@babel/runtime/helpers/esm/possibleConstructorReturn.js",
         "../node_modules/@babel/runtime/helpers/esm/assertThisInitialized.js",
         "../node_modules/@babel/runtime/helpers/esm/setPrototypeOf.js",
@@ -7469,19 +7469,19 @@
         "import classNames from 'classnames';\nimport * as React from 'react';\nimport { useContext } from 'react';\nimport { useDropdownMenu } from '@restart/ui/DropdownMenu';\nimport useIsomorphicEffect from '@restart/hooks/useIsomorphicEffect';\nimport useMergedRefs from '@restart/hooks/useMergedRefs';\nimport warning from 'warning';\nimport DropdownContext from './DropdownContext';\nimport InputGroupContext from './InputGroupContext';\nimport NavbarContext from './NavbarContext';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport useWrappedRefWithWarning from './useWrappedRefWithWarning';\nimport { alignPropType } from './types';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nexport function getDropdownMenuPlacement(alignEnd, dropDirection, isRTL) {\n  const topStart = isRTL ? 'top-end' : 'top-start';\n  const topEnd = isRTL ? 'top-start' : 'top-end';\n  const bottomStart = isRTL ? 'bottom-end' : 'bottom-start';\n  const bottomEnd = isRTL ? 'bottom-start' : 'bottom-end';\n  const leftStart = isRTL ? 'right-start' : 'left-start';\n  const leftEnd = isRTL ? 'right-end' : 'left-end';\n  const rightStart = isRTL ? 'left-start' : 'right-start';\n  const rightEnd = isRTL ? 'left-end' : 'right-end';\n  let placement = alignEnd ? bottomEnd : bottomStart;\n  if (dropDirection === 'up') placement = alignEnd ? topEnd : topStart;else if (dropDirection === 'end') placement = alignEnd ? rightEnd : rightStart;else if (dropDirection === 'start') placement = alignEnd ? leftEnd : leftStart;else if (dropDirection === 'down-centered') placement = 'bottom';else if (dropDirection === 'up-centered') placement = 'top';\n  return placement;\n}\nconst DropdownMenu = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  className,\n  align,\n  rootCloseEvent,\n  flip = true,\n  show: showProps,\n  renderOnMount,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = 'div',\n  popperConfig,\n  variant,\n  ...props\n}, ref) => {\n  let alignEnd = false;\n  const isNavbar = useContext(NavbarContext);\n  const prefix = useBootstrapPrefix(bsPrefix, 'dropdown-menu');\n  const {\n    align: contextAlign,\n    drop,\n    isRTL\n  } = useContext(DropdownContext);\n  align = align || contextAlign;\n  const isInputGroup = useContext(InputGroupContext);\n  const alignClasses = [];\n  if (align) {\n    if (typeof align === 'object') {\n      const keys = Object.keys(align);\n      process.env.NODE_ENV !== \"production\" ? warning(keys.length === 1, 'There should only be 1 breakpoint when passing an object to `align`') : void 0;\n      if (keys.length) {\n        const brkPoint = keys[0];\n        const direction = align[brkPoint];\n\n        // .dropdown-menu-end is required for responsively aligning\n        // left in addition to align left classes.\n        alignEnd = direction === 'start';\n        alignClasses.push(`${prefix}-${brkPoint}-${direction}`);\n      }\n    } else if (align === 'end') {\n      alignEnd = true;\n    }\n  }\n  const placement = getDropdownMenuPlacement(alignEnd, drop, isRTL);\n  const [menuProps, {\n    hasShown,\n    popper,\n    show,\n    toggle\n  }] = useDropdownMenu({\n    flip,\n    rootCloseEvent,\n    show: showProps,\n    usePopper: !isNavbar && alignClasses.length === 0,\n    offset: [0, 2],\n    popperConfig,\n    placement\n  });\n  menuProps.ref = useMergedRefs(useWrappedRefWithWarning(ref, 'DropdownMenu'), menuProps.ref);\n  useIsomorphicEffect(() => {\n    // Popper's initial position for the menu is incorrect when\n    // renderOnMount=true. Need to call update() to correct it.\n    if (show) popper == null ? void 0 : popper.update();\n  }, [show]);\n  if (!hasShown && !renderOnMount && !isInputGroup) return null;\n\n  // For custom components provide additional, non-DOM, props;\n  if (typeof Component !== 'string') {\n    menuProps.show = show;\n    menuProps.close = () => toggle == null ? void 0 : toggle(false);\n    menuProps.align = align;\n  }\n  let style = props.style;\n  if (popper != null && popper.placement) {\n    // we don't need the default popper style,\n    // menus are display: none when not shown.\n    style = {\n      ...props.style,\n      ...menuProps.style\n    };\n    props['x-placement'] = popper.placement;\n  }\n  return /*#__PURE__*/_jsx(Component, {\n    ...props,\n    ...menuProps,\n    style: style\n    // Bootstrap css requires this data attrib to style responsive menus.\n    ,\n    ...((alignClasses.length || isNavbar) && {\n      'data-bs-popper': 'static'\n    }),\n    className: classNames(className, prefix, show && 'show', alignEnd && `${prefix}-end`, variant && `${prefix}-${variant}`, ...alignClasses)\n  });\n});\nDropdownMenu.displayName = 'DropdownMenu';\nexport default DropdownMenu;",
         "import classNames from 'classnames';\nimport * as React from 'react';\nimport { useButtonProps } from '@restart/ui/Button';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst Button = /*#__PURE__*/React.forwardRef(({\n  as,\n  bsPrefix,\n  variant = 'primary',\n  size,\n  active = false,\n  disabled = false,\n  className,\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'btn');\n  const [buttonProps, {\n    tagName\n  }] = useButtonProps({\n    tagName: as,\n    disabled,\n    ...props\n  });\n  const Component = tagName;\n  return /*#__PURE__*/_jsx(Component, {\n    ...buttonProps,\n    ...props,\n    ref: ref,\n    disabled: disabled,\n    className: classNames(className, prefix, active && 'active', variant && `${prefix}-${variant}`, size && `${prefix}-${size}`, props.href && disabled && 'disabled')\n  });\n});\nButton.displayName = 'Button';\nexport default Button;",
         "import useMergedRefs from '@restart/hooks/useMergedRefs';\nimport DropdownContext from '@restart/ui/DropdownContext';\nimport { useDropdownToggle } from '@restart/ui/DropdownToggle';\nimport classNames from 'classnames';\nimport * as React from 'react';\nimport { useContext } from 'react';\nimport Button from './Button';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport useWrappedRefWithWarning from './useWrappedRefWithWarning';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst DropdownToggle = /*#__PURE__*/React.forwardRef(({\n  bsPrefix,\n  split,\n  className,\n  childBsPrefix,\n  // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n  as: Component = Button,\n  ...props\n}, ref) => {\n  const prefix = useBootstrapPrefix(bsPrefix, 'dropdown-toggle');\n  const dropdownContext = useContext(DropdownContext);\n  if (childBsPrefix !== undefined) {\n    props.bsPrefix = childBsPrefix;\n  }\n  const [toggleProps] = useDropdownToggle();\n  toggleProps.ref = useMergedRefs(toggleProps.ref, useWrappedRefWithWarning(ref, 'DropdownToggle'));\n\n  // This intentionally forwards size and variant (if set) to the\n  // underlying component, to allow it to render size and style variants.\n  return /*#__PURE__*/_jsx(Component, {\n    className: classNames(className, prefix, split && `${prefix}-split`, (dropdownContext == null ? void 0 : dropdownContext.show) && 'show'),\n    ...toggleProps,\n    ...props\n  });\n});\nDropdownToggle.displayName = 'DropdownToggle';\nexport default DropdownToggle;",
         "var rHyphen = /-(.)/g;\nexport default function camelize(string) {\n  return string.replace(rHyphen, function (_, chr) {\n    return chr.toUpperCase();\n  });\n}",
         "import classNames from 'classnames';\nimport camelize from 'dom-helpers/camelize';\nimport * as React from 'react';\nimport { useBootstrapPrefix } from './ThemeProvider';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst pascalCase = str => str[0].toUpperCase() + camelize(str).slice(1);\n// TODO: emstricten & fix the typing here! `createWithBsPrefix<TElementType>...`\nexport default function createWithBsPrefix(prefix, {\n  displayName = pascalCase(prefix),\n  Component,\n  defaultProps\n} = {}) {\n  const BsComponent = /*#__PURE__*/React.forwardRef(({\n    className,\n    bsPrefix,\n    as: Tag = Component || 'div',\n    ...props\n  }, ref) => {\n    const componentProps = {\n      ...defaultProps,\n      ...props\n    };\n    const resolvedPrefix = useBootstrapPrefix(bsPrefix, prefix);\n    return /*#__PURE__*/_jsx(Tag, {\n      ref: ref,\n      className: classNames(className, resolvedPrefix),\n      ...componentProps\n    });\n  });\n  BsComponent.displayName = displayName;\n  return BsComponent;\n}",
         "import classNames from 'classnames';\nimport * as React from 'react';\nimport { useContext, useMemo } from 'react';\nimport BaseDropdown from '@restart/ui/Dropdown';\nimport { useUncontrolled } from 'uncontrollable';\nimport useEventCallback from '@restart/hooks/useEventCallback';\nimport DropdownContext from './DropdownContext';\nimport DropdownItem from './DropdownItem';\nimport DropdownMenu, { getDropdownMenuPlacement } from './DropdownMenu';\nimport DropdownToggle from './DropdownToggle';\nimport InputGroupContext from './InputGroupContext';\nimport { useBootstrapPrefix, useIsRTL } from './ThemeProvider';\nimport createWithBsPrefix from './createWithBsPrefix';\nimport { alignPropType } from './types';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst DropdownHeader = createWithBsPrefix('dropdown-header', {\n  defaultProps: {\n    role: 'heading'\n  }\n});\nconst DropdownDivider = createWithBsPrefix('dropdown-divider', {\n  Component: 'hr',\n  defaultProps: {\n    role: 'separator'\n  }\n});\nconst DropdownItemText = createWithBsPrefix('dropdown-item-text', {\n  Component: 'span'\n});\nconst Dropdown = /*#__PURE__*/React.forwardRef((pProps, ref) => {\n  const {\n    bsPrefix,\n    drop = 'down',\n    show,\n    className,\n    align = 'start',\n    onSelect,\n    onToggle,\n    focusFirstItemOnShow,\n    // Need to define the default \"as\" during prop destructuring to be compatible with styled-components github.com/react-bootstrap/react-bootstrap/issues/3595\n    as: Component = 'div',\n    navbar: _4,\n    autoClose = true,\n    ...props\n  } = useUncontrolled(pProps, {\n    show: 'onToggle'\n  });\n  const isInputGroup = useContext(InputGroupContext);\n  const prefix = useBootstrapPrefix(bsPrefix, 'dropdown');\n  const isRTL = useIsRTL();\n  const isClosingPermitted = source => {\n    // autoClose=false only permits close on button click\n    if (autoClose === false) return source === 'click';\n\n    // autoClose=inside doesn't permit close on rootClose\n    if (autoClose === 'inside') return source !== 'rootClose';\n\n    // autoClose=outside doesn't permit close on select\n    if (autoClose === 'outside') return source !== 'select';\n    return true;\n  };\n  const handleToggle = useEventCallback((nextShow, meta) => {\n    if (meta.originalEvent.currentTarget === document && (meta.source !== 'keydown' || meta.originalEvent.key === 'Escape')) meta.source = 'rootClose';\n    if (isClosingPermitted(meta.source)) onToggle == null ? void 0 : onToggle(nextShow, meta);\n  });\n  const alignEnd = align === 'end';\n  const placement = getDropdownMenuPlacement(alignEnd, drop, isRTL);\n  const contextValue = useMemo(() => ({\n    align,\n    drop,\n    isRTL\n  }), [align, drop, isRTL]);\n  const directionClasses = {\n    down: prefix,\n    'down-centered': `${prefix}-center`,\n    up: 'dropup',\n    'up-centered': 'dropup-center dropup',\n    end: 'dropend',\n    start: 'dropstart'\n  };\n  return /*#__PURE__*/_jsx(DropdownContext.Provider, {\n    value: contextValue,\n    children: /*#__PURE__*/_jsx(BaseDropdown, {\n      placement: placement,\n      show: show,\n      onSelect: onSelect,\n      onToggle: handleToggle,\n      focusFirstItemOnShow: focusFirstItemOnShow,\n      itemSelector: `.${prefix}-item:not(.disabled):not(:disabled)`,\n      children: isInputGroup ? props.children : /*#__PURE__*/_jsx(Component, {\n        ...props,\n        ref: ref,\n        className: classNames(className, show && 'show', directionClasses[drop])\n      })\n    })\n  });\n});\nDropdown.displayName = 'Dropdown';\nexport default Object.assign(Dropdown, {\n  Toggle: DropdownToggle,\n  Menu: DropdownMenu,\n  Item: DropdownItem,\n  ItemText: DropdownItemText,\n  Divider: DropdownDivider,\n  Header: DropdownHeader\n});",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n * @emails oncall+draft_js\n */\n'use strict';\n\nvar seenKeys = {};\nvar MULTIPLIER = Math.pow(2, 24);\n\nfunction generateRandomKey() {\n  var key;\n\n  while (key === undefined || seenKeys.hasOwnProperty(key) || !isNaN(+key)) {\n    key = Math.floor(Math.random() * MULTIPLIER).toString(32);\n  }\n\n  seenKeys[key] = true;\n  return key;\n}\n\nmodule.exports = generateRandomKey;",
+        "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n */\n'use strict';\n\nvar AtomicBlockUtils = require(\"./AtomicBlockUtils\");\n\nvar BlockMapBuilder = require(\"./BlockMapBuilder\");\n\nvar CharacterMetadata = require(\"./CharacterMetadata\");\n\nvar CompositeDraftDecorator = require(\"./CompositeDraftDecorator\");\n\nvar ContentBlock = require(\"./ContentBlock\");\n\nvar ContentState = require(\"./ContentState\");\n\nvar DefaultDraftBlockRenderMap = require(\"./DefaultDraftBlockRenderMap\");\n\nvar DefaultDraftInlineStyle = require(\"./DefaultDraftInlineStyle\");\n\nvar DraftEditor = require(\"./DraftEditor.react\");\n\nvar DraftEditorBlock = require(\"./DraftEditorBlock.react\");\n\nvar DraftEntity = require(\"./DraftEntity\");\n\nvar DraftModifier = require(\"./DraftModifier\");\n\nvar DraftEntityInstance = require(\"./DraftEntityInstance\");\n\nvar EditorState = require(\"./EditorState\");\n\nvar KeyBindingUtil = require(\"./KeyBindingUtil\");\n\nvar RawDraftContentState = require(\"./RawDraftContentState\");\n\nvar RichTextEditorUtil = require(\"./RichTextEditorUtil\");\n\nvar SelectionState = require(\"./SelectionState\");\n\nvar convertFromDraftStateToRaw = require(\"./convertFromDraftStateToRaw\");\n\nvar convertFromRawToDraftState = require(\"./convertFromRawToDraftState\");\n\nvar generateRandomKey = require(\"./generateRandomKey\");\n\nvar getDefaultKeyBinding = require(\"./getDefaultKeyBinding\");\n\nvar getVisibleSelectionRect = require(\"./getVisibleSelectionRect\");\n\nvar convertFromHTML = require(\"./convertFromHTMLToContentBlocks\");\n\nvar DraftPublic = {\n  Editor: DraftEditor,\n  EditorBlock: DraftEditorBlock,\n  EditorState: EditorState,\n  CompositeDecorator: CompositeDraftDecorator,\n  Entity: DraftEntity,\n  EntityInstance: DraftEntityInstance,\n  BlockMapBuilder: BlockMapBuilder,\n  CharacterMetadata: CharacterMetadata,\n  ContentBlock: ContentBlock,\n  ContentState: ContentState,\n  RawDraftContentState: RawDraftContentState,\n  SelectionState: SelectionState,\n  AtomicBlockUtils: AtomicBlockUtils,\n  KeyBindingUtil: KeyBindingUtil,\n  Modifier: DraftModifier,\n  RichUtils: RichTextEditorUtil,\n  DefaultDraftBlockRenderMap: DefaultDraftBlockRenderMap,\n  DefaultDraftInlineStyle: DefaultDraftInlineStyle,\n  convertFromHTML: convertFromHTML,\n  convertFromRaw: convertFromRawToDraftState,\n  convertToRaw: convertFromDraftStateToRaw,\n  genKey: generateRandomKey,\n  getDefaultKeyBinding: getDefaultKeyBinding,\n  getVisibleSelectionRect: getVisibleSelectionRect\n};\nmodule.exports = DraftPublic;",
         "/*\nobject-assign\n(c) Sindre Sorhus\n@license MIT\n*/\n\n'use strict';\n/* eslint-disable no-unused-vars */\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar hasOwnProperty = Object.prototype.hasOwnProperty;\nvar propIsEnumerable = Object.prototype.propertyIsEnumerable;\n\nfunction toObject(val) {\n\tif (val === null || val === undefined) {\n\t\tthrow new TypeError('Object.assign cannot be called with null or undefined');\n\t}\n\n\treturn Object(val);\n}\n\nfunction shouldUseNative() {\n\ttry {\n\t\tif (!Object.assign) {\n\t\t\treturn false;\n\t\t}\n\n\t\t// Detect buggy property enumeration order in older V8 versions.\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=4118\n\t\tvar test1 = new String('abc');  // eslint-disable-line no-new-wrappers\n\t\ttest1[5] = 'de';\n\t\tif (Object.getOwnPropertyNames(test1)[0] === '5') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test2 = {};\n\t\tfor (var i = 0; i < 10; i++) {\n\t\t\ttest2['_' + String.fromCharCode(i)] = i;\n\t\t}\n\t\tvar order2 = Object.getOwnPropertyNames(test2).map(function (n) {\n\t\t\treturn test2[n];\n\t\t});\n\t\tif (order2.join('') !== '0123456789') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test3 = {};\n\t\t'abcdefghijklmnopqrst'.split('').forEach(function (letter) {\n\t\t\ttest3[letter] = letter;\n\t\t});\n\t\tif (Object.keys(Object.assign({}, test3)).join('') !==\n\t\t\t\t'abcdefghijklmnopqrst') {\n\t\t\treturn false;\n\t\t}\n\n\t\treturn true;\n\t} catch (err) {\n\t\t// We don't expect any of the above to throw, but better to be safe.\n\t\treturn false;\n\t}\n}\n\nmodule.exports = shouldUseNative() ? Object.assign : function (target, source) {\n\tvar from;\n\tvar to = toObject(target);\n\tvar symbols;\n\n\tfor (var s = 1; s < arguments.length; s++) {\n\t\tfrom = Object(arguments[s]);\n\n\t\tfor (var key in from) {\n\t\t\tif (hasOwnProperty.call(from, key)) {\n\t\t\t\tto[key] = from[key];\n\t\t\t}\n\t\t}\n\n\t\tif (getOwnPropertySymbols) {\n\t\t\tsymbols = getOwnPropertySymbols(from);\n\t\t\tfor (var i = 0; i < symbols.length; i++) {\n\t\t\t\tif (propIsEnumerable.call(from, symbols[i])) {\n\t\t\t\t\tto[symbols[i]] = from[symbols[i]];\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\t}\n\n\treturn to;\n};\n",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n * @emails oncall+draft_js\n */\n'use strict';\n\nvar KEY_DELIMITER = '-';\nvar DraftOffsetKey = {\n  encode: function encode(blockKey, decoratorKey, leafKey) {\n    return blockKey + KEY_DELIMITER + decoratorKey + KEY_DELIMITER + leafKey;\n  },\n  decode: function decode(offsetKey) {\n    // Extracts the last two parts of offsetKey and captures the rest in blockKeyParts\n    var _offsetKey$split$reve = offsetKey.split(KEY_DELIMITER).reverse(),\n        leafKey = _offsetKey$split$reve[0],\n        decoratorKey = _offsetKey$split$reve[1],\n        blockKeyParts = _offsetKey$split$reve.slice(2);\n\n    return {\n      // Recomposes the parts of blockKey after reversing them\n      blockKey: blockKeyParts.reverse().join(KEY_DELIMITER),\n      decoratorKey: parseInt(decoratorKey, 10),\n      leafKey: parseInt(leafKey, 10)\n    };\n  }\n};\nmodule.exports = DraftOffsetKey;",
         "export default function _typeof(obj) {\n  \"@babel/helpers - typeof\";\n\n  return _typeof = \"function\" == typeof Symbol && \"symbol\" == typeof Symbol.iterator ? function (obj) {\n    return typeof obj;\n  } : function (obj) {\n    return obj && \"function\" == typeof Symbol && obj.constructor === Symbol && obj !== Symbol.prototype ? \"symbol\" : typeof obj;\n  }, _typeof(obj);\n}",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n */\n'use strict';\n\nmodule.exports = function (name) {\n  if (typeof window !== 'undefined' && window.__DRAFT_GKX) {\n    return !!window.__DRAFT_GKX[name];\n  }\n\n  return false;\n};",
-        "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n */\n'use strict';\n\nvar AtomicBlockUtils = require(\"./AtomicBlockUtils\");\n\nvar BlockMapBuilder = require(\"./BlockMapBuilder\");\n\nvar CharacterMetadata = require(\"./CharacterMetadata\");\n\nvar CompositeDraftDecorator = require(\"./CompositeDraftDecorator\");\n\nvar ContentBlock = require(\"./ContentBlock\");\n\nvar ContentState = require(\"./ContentState\");\n\nvar DefaultDraftBlockRenderMap = require(\"./DefaultDraftBlockRenderMap\");\n\nvar DefaultDraftInlineStyle = require(\"./DefaultDraftInlineStyle\");\n\nvar DraftEditor = require(\"./DraftEditor.react\");\n\nvar DraftEditorBlock = require(\"./DraftEditorBlock.react\");\n\nvar DraftEntity = require(\"./DraftEntity\");\n\nvar DraftModifier = require(\"./DraftModifier\");\n\nvar DraftEntityInstance = require(\"./DraftEntityInstance\");\n\nvar EditorState = require(\"./EditorState\");\n\nvar KeyBindingUtil = require(\"./KeyBindingUtil\");\n\nvar RawDraftContentState = require(\"./RawDraftContentState\");\n\nvar RichTextEditorUtil = require(\"./RichTextEditorUtil\");\n\nvar SelectionState = require(\"./SelectionState\");\n\nvar convertFromDraftStateToRaw = require(\"./convertFromDraftStateToRaw\");\n\nvar convertFromRawToDraftState = require(\"./convertFromRawToDraftState\");\n\nvar generateRandomKey = require(\"./generateRandomKey\");\n\nvar getDefaultKeyBinding = require(\"./getDefaultKeyBinding\");\n\nvar getVisibleSelectionRect = require(\"./getVisibleSelectionRect\");\n\nvar convertFromHTML = require(\"./convertFromHTMLToContentBlocks\");\n\nvar DraftPublic = {\n  Editor: DraftEditor,\n  EditorBlock: DraftEditorBlock,\n  EditorState: EditorState,\n  CompositeDecorator: CompositeDraftDecorator,\n  Entity: DraftEntity,\n  EntityInstance: DraftEntityInstance,\n  BlockMapBuilder: BlockMapBuilder,\n  CharacterMetadata: CharacterMetadata,\n  ContentBlock: ContentBlock,\n  ContentState: ContentState,\n  RawDraftContentState: RawDraftContentState,\n  SelectionState: SelectionState,\n  AtomicBlockUtils: AtomicBlockUtils,\n  KeyBindingUtil: KeyBindingUtil,\n  Modifier: DraftModifier,\n  RichUtils: RichTextEditorUtil,\n  DefaultDraftBlockRenderMap: DefaultDraftBlockRenderMap,\n  DefaultDraftInlineStyle: DefaultDraftInlineStyle,\n  convertFromHTML: convertFromHTML,\n  convertFromRaw: convertFromRawToDraftState,\n  convertToRaw: convertFromDraftStateToRaw,\n  genKey: generateRandomKey,\n  getDefaultKeyBinding: getDefaultKeyBinding,\n  getVisibleSelectionRect: getVisibleSelectionRect\n};\nmodule.exports = DraftPublic;",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n * @emails oncall+draft_js\n */\n'use strict';\n\nfunction _inheritsLoose(subClass, superClass) { subClass.prototype = Object.create(superClass.prototype); subClass.prototype.constructor = subClass; subClass.__proto__ = superClass; }\n\nvar CharacterMetadata = require(\"./CharacterMetadata\");\n\nvar findRangesImmutable = require(\"./findRangesImmutable\");\n\nvar Immutable = require(\"immutable\");\n\nvar List = Immutable.List,\n    Map = Immutable.Map,\n    OrderedSet = Immutable.OrderedSet,\n    Record = Immutable.Record,\n    Repeat = Immutable.Repeat;\nvar EMPTY_SET = OrderedSet();\nvar defaultRecord = {\n  key: '',\n  type: 'unstyled',\n  text: '',\n  characterList: List(),\n  depth: 0,\n  data: Map()\n};\nvar ContentBlockRecord = Record(defaultRecord);\n\nvar decorateCharacterList = function decorateCharacterList(config) {\n  if (!config) {\n    return config;\n  }\n\n  var characterList = config.characterList,\n      text = config.text;\n\n  if (text && !characterList) {\n    config.characterList = List(Repeat(CharacterMetadata.EMPTY, text.length));\n  }\n\n  return config;\n};\n\nvar ContentBlock = /*#__PURE__*/function (_ContentBlockRecord) {\n  _inheritsLoose(ContentBlock, _ContentBlockRecord);\n\n  function ContentBlock(config) {\n    return _ContentBlockRecord.call(this, decorateCharacterList(config)) || this;\n  }\n\n  var _proto = ContentBlock.prototype;\n\n  _proto.getKey = function getKey() {\n    return this.get('key');\n  };\n\n  _proto.getType = function getType() {\n    return this.get('type');\n  };\n\n  _proto.getText = function getText() {\n    return this.get('text');\n  };\n\n  _proto.getCharacterList = function getCharacterList() {\n    return this.get('characterList');\n  };\n\n  _proto.getLength = function getLength() {\n    return this.getText().length;\n  };\n\n  _proto.getDepth = function getDepth() {\n    return this.get('depth');\n  };\n\n  _proto.getData = function getData() {\n    return this.get('data');\n  };\n\n  _proto.getInlineStyleAt = function getInlineStyleAt(offset) {\n    var character = this.getCharacterList().get(offset);\n    return character ? character.getStyle() : EMPTY_SET;\n  };\n\n  _proto.getEntityAt = function getEntityAt(offset) {\n    var character = this.getCharacterList().get(offset);\n    return character ? character.getEntity() : null;\n  }\n  /**\n   * Execute a callback for every contiguous range of styles within the block.\n   */\n  ;\n\n  _proto.findStyleRanges = function findStyleRanges(filterFn, callback) {\n    findRangesImmutable(this.getCharacterList(), haveEqualStyle, filterFn, callback);\n  }\n  /**\n   * Execute a callback for every contiguous range of entities within the block.\n   */\n  ;\n\n  _proto.findEntityRanges = function findEntityRanges(filterFn, callback) {\n    findRangesImmutable(this.getCharacterList(), haveEqualEntity, filterFn, callback);\n  };\n\n  return ContentBlock;\n}(ContentBlockRecord);\n\nfunction haveEqualStyle(charA, charB) {\n  return charA.getStyle() === charB.getStyle();\n}\n\nfunction haveEqualEntity(charA, charB) {\n  return charA.getEntity() === charB.getEntity();\n}\n\nmodule.exports = ContentBlock;",
         "\"use strict\";\n\n/**\n * Copyright (c) 2013-present, Facebook, Inc.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n */\n\n/**\n * This function is used to mark string literals representing CSS class names\n * so that they can be transformed statically. This allows for modularization\n * and minification of CSS class names.\n *\n * In static_upstream, this function is actually implemented, but it should\n * eventually be replaced with something more descriptive, and the transform\n * that is used in the main stack should be ported for use elsewhere.\n *\n * @param string|object className to modularize, or an object of key/values.\n *                      In the object case, the values are conditions that\n *                      determine if the className keys should be included.\n * @param [string ...]  Variable list of classNames in the string case.\n * @return string       Renderable space-separated CSS className.\n */\nfunction cx(classNames) {\n  if (typeof classNames == 'object') {\n    return Object.keys(classNames).filter(function (className) {\n      return classNames[className];\n    }).map(replace).join(' ');\n  }\n\n  return Array.prototype.map.call(arguments, replace).join(' ');\n}\n\nfunction replace(str) {\n  return str.replace(/\\//g, '-');\n}\n\nmodule.exports = cx;",
         "\"use strict\";\n\n/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @format\n * \n * @emails oncall+draft_js\n */\nfunction isElement(node) {\n  if (!node || !node.ownerDocument) {\n    return false;\n  }\n\n  return node.nodeType === Node.ELEMENT_NODE;\n}\n\nmodule.exports = isElement;",
         "/**\n * Copyright (c) 2013-present, Facebook, Inc.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @typechecks\n */\n\n/**\n * Unicode-enabled replacesments for basic String functions.\n *\n * All the functions in this module assume that the input string is a valid\n * UTF-16 encoding of a Unicode sequence. If it's not the case, the behavior\n * will be undefined.\n *\n * WARNING: Since this module is typechecks-enforced, you may find new bugs\n * when replacing normal String functions with ones provided here.\n */\n'use strict';\n\nvar invariant = require(\"./invariant\"); // These two ranges are consecutive so anything in [HIGH_START, LOW_END] is a\n// surrogate code unit.\n\n\nvar SURROGATE_HIGH_START = 0xD800;\nvar SURROGATE_HIGH_END = 0xDBFF;\nvar SURROGATE_LOW_START = 0xDC00;\nvar SURROGATE_LOW_END = 0xDFFF;\nvar SURROGATE_UNITS_REGEX = /[\\uD800-\\uDFFF]/;\n/**\n * @param {number} codeUnit   A Unicode code-unit, in range [0, 0x10FFFF]\n * @return {boolean}          Whether code-unit is in a surrogate (hi/low) range\n */\n\nfunction isCodeUnitInSurrogateRange(codeUnit) {\n  return SURROGATE_HIGH_START <= codeUnit && codeUnit <= SURROGATE_LOW_END;\n}\n/**\n * Returns whether the two characters starting at `index` form a surrogate pair.\n * For example, given the string s = \"\\uD83D\\uDE0A\", (s, 0) returns true and\n * (s, 1) returns false.\n *\n * @param {string} str\n * @param {number} index\n * @return {boolean}\n */\n\n\nfunction isSurrogatePair(str, index) {\n  !(0 <= index && index < str.length) ? process.env.NODE_ENV !== \"production\" ? invariant(false, 'isSurrogatePair: Invalid index %s for string length %s.', index, str.length) : invariant(false) : void 0;\n\n  if (index + 1 === str.length) {\n    return false;\n  }\n\n  var first = str.charCodeAt(index);\n  var second = str.charCodeAt(index + 1);\n  return SURROGATE_HIGH_START <= first && first <= SURROGATE_HIGH_END && SURROGATE_LOW_START <= second && second <= SURROGATE_LOW_END;\n}\n/**\n * @param {string} str  Non-empty string\n * @return {boolean}    True if the input includes any surrogate code units\n */\n\n\nfunction hasSurrogateUnit(str) {\n  return SURROGATE_UNITS_REGEX.test(str);\n}\n/**\n * Return the length of the original Unicode character at given position in the\n * String by looking into the UTF-16 code unit; that is equal to 1 for any\n * non-surrogate characters in BMP ([U+0000..U+D7FF] and [U+E000, U+FFFF]); and\n * returns 2 for the hi/low surrogates ([U+D800..U+DFFF]), which are in fact\n * representing non-BMP characters ([U+10000..U+10FFFF]).\n *\n * Examples:\n * - '\\u0020' => 1\n * - '\\u3020' => 1\n * - '\\uD835' => 2\n * - '\\uD835\\uDDEF' => 2\n * - '\\uDDEF' => 2\n *\n * @param {string} str  Non-empty string\n * @param {number} pos  Position in the string to look for one code unit\n * @return {number}      Number 1 or 2\n */\n\n\nfunction getUTF16Length(str, pos) {\n  return 1 + isCodeUnitInSurrogateRange(str.charCodeAt(pos));\n}\n/**\n * Fully Unicode-enabled replacement for String#length\n *\n * @param {string} str  Valid Unicode string\n * @return {number}     The number of Unicode characters in the string\n */\n\n\nfunction strlen(str) {\n  // Call the native functions if there's no surrogate char\n  if (!hasSurrogateUnit(str)) {\n    return str.length;\n  }\n\n  var len = 0;\n\n  for (var pos = 0; pos < str.length; pos += getUTF16Length(str, pos)) {\n    len++;\n  }\n\n  return len;\n}\n/**\n * Fully Unicode-enabled replacement for String#substr()\n *\n * @param {string} str      Valid Unicode string\n * @param {number} start    Location in Unicode sequence to begin extracting\n * @param {?number} length  The number of Unicode characters to extract\n *                          (default: to the end of the string)\n * @return {string}         Extracted sub-string\n */\n\n\nfunction substr(str, start, length) {\n  start = start || 0;\n  length = length === undefined ? Infinity : length || 0; // Call the native functions if there's no surrogate char\n\n  if (!hasSurrogateUnit(str)) {\n    return str.substr(start, length);\n  } // Obvious cases\n\n\n  var size = str.length;\n\n  if (size <= 0 || start > size || length <= 0) {\n    return '';\n  } // Find the actual starting position\n\n\n  var posA = 0;\n\n  if (start > 0) {\n    for (; start > 0 && posA < size; start--) {\n      posA += getUTF16Length(str, posA);\n    }\n\n    if (posA >= size) {\n      return '';\n    }\n  } else if (start < 0) {\n    for (posA = size; start < 0 && 0 < posA; start++) {\n      posA -= getUTF16Length(str, posA - 1);\n    }\n\n    if (posA < 0) {\n      posA = 0;\n    }\n  } // Find the actual ending position\n\n\n  var posB = size;\n\n  if (length < size) {\n    for (posB = posA; length > 0 && posB < size; length--) {\n      posB += getUTF16Length(str, posB);\n    }\n  }\n\n  return str.substring(posA, posB);\n}\n/**\n * Fully Unicode-enabled replacement for String#substring()\n *\n * @param {string} str    Valid Unicode string\n * @param {number} start  Location in Unicode sequence to begin extracting\n * @param {?number} end   Location in Unicode sequence to end extracting\n *                        (default: end of the string)\n * @return {string}       Extracted sub-string\n */\n\n\nfunction substring(str, start, end) {\n  start = start || 0;\n  end = end === undefined ? Infinity : end || 0;\n\n  if (start < 0) {\n    start = 0;\n  }\n\n  if (end < 0) {\n    end = 0;\n  }\n\n  var length = Math.abs(end - start);\n  start = start < end ? start : end;\n  return substr(str, start, length);\n}\n/**\n * Get a list of Unicode code-points from a String\n *\n * @param {string} str        Valid Unicode string\n * @return {array<number>}    A list of code-points in [0..0x10FFFF]\n */\n\n\nfunction getCodePoints(str) {\n  var codePoints = [];\n\n  for (var pos = 0; pos < str.length; pos += getUTF16Length(str, pos)) {\n    codePoints.push(str.codePointAt(pos));\n  }\n\n  return codePoints;\n}\n\nvar UnicodeUtils = {\n  getCodePoints: getCodePoints,\n  getUTF16Length: getUTF16Length,\n  hasSurrogateUnit: hasSurrogateUnit,\n  isCodeUnitInSurrogateRange: isCodeUnitInSurrogateRange,\n  isSurrogatePair: isSurrogatePair,\n  strlen: strlen,\n  substring: substring,\n  substr: substr\n};\nmodule.exports = UnicodeUtils;",
         "import _typeof from \"./typeof.js\";\nimport assertThisInitialized from \"./assertThisInitialized.js\";\nexport default function _possibleConstructorReturn(self, call) {\n  if (call && (_typeof(call) === \"object\" || typeof call === \"function\")) {\n    return call;\n  } else if (call !== void 0) {\n    throw new TypeError(\"Derived constructors may only return object or undefined\");\n  }\n  return assertThisInitialized(self);\n}",
         "export default function _assertThisInitialized(self) {\n  if (self === void 0) {\n    throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\");\n  }\n  return self;\n}",
         "export default function _setPrototypeOf(o, p) {\n  _setPrototypeOf = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function _setPrototypeOf(o, p) {\n    o.__proto__ = p;\n    return o;\n  };\n  return _setPrototypeOf(o, p);\n}",
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,159 +1,159 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
         216: function(e, t, n) {},
         218: function(e, t, n) {
             "use strict";
             n.r(t);
             var r = n(4),
-                o = n.n(r),
-                a = n(68),
-                c = n.n(a),
+                a = n.n(r),
+                o = n(68),
+                c = n.n(o),
                 i = n(0),
                 s = n(1),
                 l = n(2),
                 d = n(3),
                 u = n(45),
-                p = n(28),
+                p = n(24),
                 b = n(109),
                 j = (n(215), n(216), n(22)),
                 h = n(110),
                 m = n.n(h),
-                g = n(7),
-                v = function(e) {
+                v = n(7),
+                g = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n() {
                         var e;
                         Object(i.a)(this, n);
-                        for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
-                        return (e = t.call.apply(t, [this].concat(o))).addStar = function(t) {
+                        for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
+                        return (e = t.call.apply(t, [this].concat(a))).addStar = function(t) {
                             var n = e.props,
                                 r = n.editorState,
-                                o = n.onChange,
-                                a = p.Modifier.replaceText(r.getCurrentContent(), r.getSelection(), "{df['".concat(t, "']"), r.getCurrentInlineStyle());
-                            o(p.EditorState.push(r, a, "insert-characters"))
+                                a = n.onChange,
+                                o = p.Modifier.replaceText(r.getCurrentContent(), r.getSelection(), "{df['".concat(t, "']"), r.getCurrentInlineStyle());
+                            a(p.EditorState.push(r, o, "insert-characters"))
                         }, e
                     }
                     return Object(s.a)(n, [{
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = this.props.column;
-                            return Object(g.jsx)("div", {
+                            return Object(v.jsx)("div", {
                                 style: {
                                     padding: "0 3px"
                                 },
-                                children: Object(g.jsxs)(j.a, {
-                                    children: [Object(g.jsx)(j.a.Toggle, {
+                                children: Object(v.jsxs)(j.a, {
+                                    children: [Object(v.jsx)(j.a.Toggle, {
                                         variant: "primary",
                                         id: "dropdown-basic",
                                         children: "Select Variable"
-                                    }), Object(g.jsxs)(j.a.Menu, {
+                                    }), Object(v.jsxs)(j.a.Menu, {
                                         style: {
                                             maxHeight: "150px",
                                             overflowY: "auto",
                                             columnCount: 2
                                         },
-                                        children: [Object(g.jsx)("div", {
+                                        children: [Object(v.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 0 ? Object(g.jsx)(j.a.Item, {
+                                                return n % 2 === 0 ? Object(v.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
-                                        }), Object(g.jsx)("div", {
+                                        }), Object(v.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 1 ? Object(g.jsx)(j.a.Item, {
+                                                return n % 2 === 1 ? Object(v.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
                                         })]
                                     })]
                                 })
                             })
                         }
                     }]), n
                 }(r.Component),
-                f = function(e) {
+                C = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n() {
                         var e;
                         Object(i.a)(this, n);
-                        for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
-                        return (e = t.call.apply(t, [this].concat(o))).addStar = function(t) {
+                        for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
+                        return (e = t.call.apply(t, [this].concat(a))).addStar = function(t) {
                             var n = e.props,
                                 r = n.editorState,
-                                o = n.onChange,
-                                a = p.Modifier.replaceText(r.getCurrentContent(), r.getSelection(), ".".concat(t, "()}"), r.getCurrentInlineStyle());
-                            o(p.EditorState.push(r, a, "insert-characters"))
+                                a = n.onChange,
+                                o = p.Modifier.replaceText(r.getCurrentContent(), r.getSelection(), ".".concat(t, "()}"), r.getCurrentInlineStyle());
+                            a(p.EditorState.push(r, o, "insert-characters"))
                         }, e
                     }
                     return Object(s.a)(n, [{
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = this.props.agg;
-                            return Object(g.jsx)("div", {
+                            return Object(v.jsx)("div", {
                                 style: {
                                     padding: "0 3px"
                                 },
-                                children: Object(g.jsxs)(j.a, {
-                                    children: [Object(g.jsx)(j.a.Toggle, {
+                                children: Object(v.jsxs)(j.a, {
+                                    children: [Object(v.jsx)(j.a.Toggle, {
                                         variant: "primary",
                                         id: "dropdown-basic",
                                         children: "Select Aggregate"
-                                    }), Object(g.jsxs)(j.a.Menu, {
+                                    }), Object(v.jsxs)(j.a.Menu, {
                                         style: {
                                             maxHeight: "150px",
                                             overflowY: "auto",
                                             columnCount: 2
                                         },
-                                        children: [Object(g.jsx)("div", {
+                                        children: [Object(v.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 0 ? Object(g.jsx)(j.a.Item, {
+                                                return n % 2 === 0 ? Object(v.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
-                                        }), Object(g.jsx)("div", {
+                                        }), Object(v.jsx)("div", {
                                             children: t.map((function(t, n) {
-                                                return n % 2 === 1 ? Object(g.jsx)(j.a.Item, {
+                                                return n % 2 === 1 ? Object(v.jsx)(j.a.Item, {
                                                     onClick: function() {
                                                         return e.addStar(t)
                                                     },
                                                     children: t
                                                 }, t) : null
                                             }))
                                         })]
                                     })]
                                 })
                             })
                         }
                     }]), n
                 }(r.Component),
-                O = function(e) {
+                f = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n() {
                         var e;
                         Object(i.a)(this, n);
-                        for (var r = arguments.length, o = new Array(r), a = 0; a < r; a++) o[a] = arguments[a];
-                        return (e = t.call.apply(t, [this].concat(o))).state = {
+                        for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
+                        return (e = t.call.apply(t, [this].concat(a))).state = {
                             isHovered: !1
                         }, e.onButtonClicked = function() {
                             var t = e.props.editorState,
                                 n = m()(Object(p.convertToRaw)(t.getCurrentContent())),
                                 r = t.getCurrentContent().getPlainText("\x01");
                             u.a.setComponentValue([!0, n, r])
                         }, e.handleMouseEnter = function() {
@@ -174,36 +174,36 @@
                                     backgroundColor: "initial",
                                     color: e ? "#FF4B4B" : "black",
                                     border: "1px solid ".concat(e ? "red" : "#F0F2F6"),
                                     borderRadius: "5px",
                                     padding: "5px 8px",
                                     transition: "background-color 0.1s ease"
                                 };
-                            return Object(g.jsx)("div", {
+                            return Object(v.jsx)("div", {
                                 style: {
                                     marginTop: "10px"
                                 },
-                                children: Object(g.jsx)("button", {
+                                children: Object(v.jsx)("button", {
                                     style: t,
                                     onMouseEnter: this.handleMouseEnter,
                                     onMouseLeave: this.handleMouseLeave,
                                     onClick: this.onButtonClicked,
                                     children: "Confirm Text"
                                 })
                             })
                         }
                     }]), n
-                }(o.a.Component),
+                }(a.a.Component),
                 x = function(e) {
                     Object(l.a)(n, e);
                     var t = Object(d.a)(n);
 
                     function n(e) {
                         var r;
-                        return Object(i.a)(this, n), (r = t.call(this, e)).onClicked = function() {
+                        Object(i.a)(this, n), (r = t.call(this, e)).onClicked = function() {
                             r.setState((function(e) {
                                 return {
                                     numClicks: e.numClicks + 1
                                 }
                             }), (function() {
                                 return u.a.setComponentValue(r.state.numClicks)
                             }))
@@ -215,42 +215,44 @@
                             r.setState({
                                 isFocused: !1
                             })
                         }, r.handleEditorChange = function(e) {
                             r.setState({
                                 editorState: e
                             })
-                        }, r.state = {
+                        };
+                        var a = e.args.value;
+                        return r.state = {
                             numClicks: 0,
                             isFocused: !1,
-                            editorState: p.EditorState.createEmpty()
+                            editorState: a ? p.EditorState.createWithContent(p.ContentState.createFromText(a)) : p.EditorState.createEmpty()
                         }, r
                     }
                     return Object(s.a)(n, [{
                         key: "render",
                         value: function() {
                             var e = this.props.args,
                                 t = this.state.editorState,
                                 n = e.placeholder,
                                 r = e.columns,
-                                o = e.agg;
-                            return Object(g.jsxs)("div", {
+                                a = e.agg;
+                            return Object(v.jsxs)("div", {
                                 style: {
                                     position: "relative"
                                 },
-                                children: [Object(g.jsx)(b.Editor, {
+                                children: [Object(v.jsx)(b.Editor, {
                                     editorState: t,
                                     onEditorStateChange: this.handleEditorChange,
                                     wrapperClassName: "wrapper-class",
                                     editorClassName: "editor-class",
                                     toolbarClassName: "toolbar-class",
-                                    toolbarCustomButtons: [Object(g.jsx)(v, {
+                                    toolbarCustomButtons: [Object(v.jsx)(g, {
                                         column: r
-                                    }), Object(g.jsx)(f, {
-                                        agg: o
+                                    }), Object(v.jsx)(C, {
+                                        agg: a
                                     })],
                                     placeholder: n,
                                     toolbar: {
                                         options: ["inline", "blockType", "colorPicker"],
                                         inline: {
                                             options: ["bold", "italic", "underline"],
                                             bold: {
@@ -271,25 +273,25 @@
                                         },
                                         colorPicker: {
                                             component: void 0,
                                             popupClassName: void 0,
                                             colors: ["rgb(0, 0, 0)", "rgb(255, 0, 0)", "rgb(0, 255, 0)", "rgb(0, 0, 255)", "rgb(255, 255, 0)", "rgb(255, 255, 255)"]
                                         }
                                     }
-                                }), Object(g.jsx)(O, {
+                                }), Object(v.jsx)(f, {
                                     editorState: t
                                 })]
                             })
                         }
                     }]), n
                 }(u.b),
-                C = Object(u.c)(x);
-            c.a.render(Object(g.jsx)(o.a.StrictMode, {
-                children: Object(g.jsx)(C, {})
+                O = Object(u.c)(x);
+            c.a.render(Object(v.jsx)(a.a.StrictMode, {
+                children: Object(v.jsx)(O, {})
             }), document.getElementById("root"))
         }
     },
     [
         [218, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.baa131a3.chunk.js.map
+//# sourceMappingURL=main.7e37a4e5.chunk.js.map
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8074683110654334%*

 * *Differences: {"'file'": "'static/js/main.7e37a4e5.chunk.js'",*

 * * "'mappings'": "'sTAeMA,EAAmB,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GAgBrB,OAhBqBP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KAOvBM,QAAU,SAACC,GACT,IAAAC,EAAkCb,EAAKc,MAA/BC,EAAWF,EAAXE,YAAaC,EAAQH,EAARG,SACfC,EAAeC,WAASC,YAC5BJ,EAAYK,oBACZL,EAAYM,eAAe,QAADX,OAClBE,EAAU,MAClBG,EAAYO,yBAEdN,EAASO,cAAYC,KAAKT,EAAaE,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.baa131a3.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.7e37a4e5.chunk.js",
+    "mappings": "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",
     "names": [
         "FirstDropdownOption",
         "_Component",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -102,14 +102,18 @@
         "onClicked",
         "prevState",
         "numClicks",
         "onFocus",
         "isFocused",
         "onBlur",
         "handleEditorChange",
+        "initialValue",
+        "createWithContent",
+        "ContentState",
+        "createFromText",
         "createEmpty",
         "placeholder",
         "columns",
         "position",
         "Editor",
         "onEditorStateChange",
         "wrapperClassName",
@@ -140,12 +144,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "PandasTextEditor.js",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\";\r\nimport React, { Component } from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport { EditorState, Modifier, convertToRaw } from 'draft-js';\r\nimport { Editor } from 'react-draft-wysiwyg';\r\nimport \"react-draft-wysiwyg/dist/react-draft-wysiwyg.css\";\r\nimport './app.css';\r\nimport Dropdown from 'react-bootstrap/Dropdown';\r\nimport draftToHtml from \"draftjs-to-html\";\r\n\r\n// first choice dropdown\r\nclass FirstDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    column: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (columnName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `{df['${columnName}']`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { column } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Variable\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// second dropdown choice\r\nclass SecondDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    agg: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (aggName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `.${aggName}()}`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { agg } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Aggregate\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// my custom react button to emulate the streamlit button\r\nclass Button extends React.Component {\r\n  state = {\r\n    isHovered: false\r\n  };\r\n\r\n  onButtonClicked = () => {\r\n    const { editorState } = this.props;\r\n    const content = draftToHtml(convertToRaw(editorState.getCurrentContent()));\r\n    const contentState = editorState.getCurrentContent()\r\n    const contentPlainText = contentState.getPlainText('\\u0001');\r\n    Streamlit.setComponentValue([true, content, contentPlainText]);\r\n  };\r\n\r\n  handleMouseEnter = () => {\r\n    this.setState({ isHovered: true });\r\n  };\r\n\r\n  handleMouseLeave = () => {\r\n    this.setState({ isHovered: false });\r\n  };\r\n\r\n  render() {\r\n    const { isHovered } = this.state;\r\n    const buttonContainerStyle = {\r\n      marginTop: '10px', // Adjust the value as needed\r\n    };\r\n    const buttonStyle = {\r\n      backgroundColor: 'initial',\r\n      color: isHovered ? '#FF4B4B' : 'black',\r\n      border: `1px solid ${isHovered ? 'red' : '#F0F2F6'}`,\r\n      borderRadius: '5px',\r\n      padding: '5px 8px',\r\n      transition: 'background-color 0.1s ease',\r\n      // Add other styles here\r\n    };\r\n\r\n    return (\r\n      <div style={buttonContainerStyle}>\r\n        <button\r\n          style={buttonStyle}\r\n          onMouseEnter={this.handleMouseEnter}\r\n          onMouseLeave={this.handleMouseLeave}\r\n          onClick={this.onButtonClicked}\r\n        >\r\n          Confirm Text\r\n        </button>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// main component\r\nclass PandasTextEditor extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props);\r\n\r\n    this.state = {\r\n      numClicks: 0,\r\n      isFocused: false,\r\n      editorState: EditorState.createEmpty(), // Initialize the editor state\r\n    };\r\n  }\r\n\r\n  onClicked = () => {\r\n    this.setState(\r\n      (prevState) => ({ numClicks: prevState.numClicks + 1 }),\r\n      () => Streamlit.setComponentValue(this.state.numClicks)\r\n    );\r\n  };\r\n\r\n  onFocus = () => {\r\n    this.setState({ isFocused: true });\r\n  };\r\n\r\n  onBlur = () => {\r\n    this.setState({ isFocused: false });\r\n  };\r\n\r\n  handleEditorChange = (editorState) => {\r\n    this.setState({ editorState });\r\n  };\r\n\r\n  render() {\r\n    const { args } = this.props;\r\n    const { editorState } = this.state;\r\n    const placeholder = args[\"placeholder\"];\r\n\r\n    const columns = args[\"columns\"];\r\n    const agg = args[\"agg\"];\r\n\r\n    return (\r\n      <div style={{ position: \"relative\" }}>\r\n        <Editor\r\n          editorState={editorState}\r\n          onEditorStateChange={this.handleEditorChange}\r\n          wrapperClassName=\"wrapper-class\"\r\n          editorClassName=\"editor-class\"\r\n          toolbarClassName=\"toolbar-class\"\r\n          toolbarCustomButtons={[<FirstDropdownOption column={columns} />, <SecondDropdownOption agg={agg} />]}\r\n          placeholder={placeholder}\r\n          toolbar={{\r\n            options: ['inline', 'blockType', 'colorPicker'],\r\n            inline: {\r\n              options: ['bold', 'italic', 'underline'],\r\n              bold: { className: 'bordered-option-classname' },\r\n              italic: { className: 'bordered-option-classname' },\r\n              underline: { className: 'bordered-option-classname' },\r\n            },\r\n            blockType: {\r\n              inDropdown: true,\r\n              maxHeight: \"100px\", overflowY: \"auto\", columnCount: 2\r\n            },\r\n            colorPicker: {\r\n              component: undefined,\r\n              popupClassName: undefined,\r\n              colors: ['rgb(0, 0, 0)',\r\n                'rgb(255, 0, 0)',   // Red\r\n                'rgb(0, 255, 0)',   // Green\r\n                'rgb(0, 0, 255)',   // Blue\r\n                'rgb(255, 255, 0)', // Yellow\r\n                'rgb(255, 255, 255)']\r\n            }\r\n          }}\r\n        />\r\n        <Button editorState={editorState} />\r\n      </div>\r\n\r\n\r\n    );\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(PandasTextEditor);",
+        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\";\r\nimport React, { Component } from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport { EditorState, Modifier, convertToRaw, ContentState } from 'draft-js';\r\nimport { Editor } from 'react-draft-wysiwyg';\r\nimport \"react-draft-wysiwyg/dist/react-draft-wysiwyg.css\";\r\nimport './app.css';\r\nimport Dropdown from 'react-bootstrap/Dropdown';\r\nimport draftToHtml from \"draftjs-to-html\";\r\n\r\n// first choice dropdown\r\nclass FirstDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    column: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (columnName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `{df['${columnName}']`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { column } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Variable\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {column.map((columnName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={columnName} onClick={() => this.addStar(columnName)}>\r\n                      {columnName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// second dropdown choice\r\nclass SecondDropdownOption extends Component {\r\n  static propTypes = {\r\n    onChange: PropTypes.func,\r\n    editorState: PropTypes.object,\r\n    agg: PropTypes.arrayOf(PropTypes.string),\r\n  };\r\n\r\n  addStar = (aggName) => {\r\n    const { editorState, onChange } = this.props;\r\n    const contentState = Modifier.replaceText(\r\n      editorState.getCurrentContent(),\r\n      editorState.getSelection(),\r\n      `.${aggName}()}`,\r\n      editorState.getCurrentInlineStyle(),\r\n    );\r\n    onChange(EditorState.push(editorState, contentState, 'insert-characters'));\r\n  };\r\n\r\n  render() {\r\n    const { agg } = this.props;\r\n\r\n    return (\r\n      <div style={{ padding: '0 3px' }}>\r\n        <Dropdown>\r\n          <Dropdown.Toggle variant=\"primary\" id=\"dropdown-basic\">\r\n            Select Aggregate\r\n          </Dropdown.Toggle>\r\n          <Dropdown.Menu style={{ maxHeight: \"150px\", overflowY: \"auto\", columnCount: 2 }}>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 0) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n            <div>\r\n              {agg.map((aggName, index) => {\r\n                if (index % 2 === 1) {\r\n                  return (\r\n                    <Dropdown.Item key={aggName} onClick={() => this.addStar(aggName)}>\r\n                      {aggName}\r\n                    </Dropdown.Item>\r\n                  );\r\n                }\r\n                return null;\r\n              })}\r\n            </div>\r\n          </Dropdown.Menu>\r\n        </Dropdown>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// my custom react button to emulate the streamlit button\r\nclass Button extends React.Component {\r\n  state = {\r\n    isHovered: false\r\n  };\r\n\r\n  onButtonClicked = () => {\r\n    const { editorState } = this.props;\r\n    const content = draftToHtml(convertToRaw(editorState.getCurrentContent()));\r\n    const contentState = editorState.getCurrentContent()\r\n    const contentPlainText = contentState.getPlainText('\\u0001');\r\n    Streamlit.setComponentValue([true, content, contentPlainText]);\r\n  };\r\n\r\n  handleMouseEnter = () => {\r\n    this.setState({ isHovered: true });\r\n  };\r\n\r\n  handleMouseLeave = () => {\r\n    this.setState({ isHovered: false });\r\n  };\r\n\r\n  render() {\r\n    const { isHovered } = this.state;\r\n    const buttonContainerStyle = {\r\n      marginTop: '10px', // Adjust the value as needed\r\n    };\r\n    const buttonStyle = {\r\n      backgroundColor: 'initial',\r\n      color: isHovered ? '#FF4B4B' : 'black',\r\n      border: `1px solid ${isHovered ? 'red' : '#F0F2F6'}`,\r\n      borderRadius: '5px',\r\n      padding: '5px 8px',\r\n      transition: 'background-color 0.1s ease',\r\n      // Add other styles here\r\n    };\r\n\r\n    return (\r\n      <div style={buttonContainerStyle}>\r\n        <button\r\n          style={buttonStyle}\r\n          onMouseEnter={this.handleMouseEnter}\r\n          onMouseLeave={this.handleMouseLeave}\r\n          onClick={this.onButtonClicked}\r\n        >\r\n          Confirm Text\r\n        </button>\r\n      </div>\r\n    );\r\n  }\r\n}\r\n\r\n// main component\r\nclass PandasTextEditor extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props);\r\n\r\n    const { args } = props;\r\n    const initialValue = args[\"value\"];\r\n\r\n    this.state = {\r\n      numClicks: 0,\r\n      isFocused: false,\r\n      // Initialize the editor state with a customValue\r\n      editorState: initialValue ? EditorState.createWithContent(ContentState.createFromText(initialValue)) : EditorState.createEmpty(),\r\n    };\r\n  }\r\n\r\n  onClicked = () => {\r\n    this.setState(\r\n      (prevState) => ({ numClicks: prevState.numClicks + 1 }),\r\n      () => Streamlit.setComponentValue(this.state.numClicks)\r\n    );\r\n  };\r\n\r\n  onFocus = () => {\r\n    this.setState({ isFocused: true });\r\n  };\r\n\r\n  onBlur = () => {\r\n    this.setState({ isFocused: false });\r\n  };\r\n\r\n  handleEditorChange = (editorState) => {\r\n    this.setState({ editorState });\r\n  };\r\n\r\n  render() {\r\n    const { args } = this.props;\r\n    const { editorState } = this.state;\r\n    const placeholder = args[\"placeholder\"];\r\n    const columns = args[\"columns\"];\r\n    const agg = args[\"agg\"];\r\n\r\n    return (\r\n      <div style={{ position: \"relative\" }}>\r\n        <Editor\r\n          editorState={editorState}\r\n          onEditorStateChange={this.handleEditorChange}\r\n          wrapperClassName=\"wrapper-class\"\r\n          editorClassName=\"editor-class\"\r\n          toolbarClassName=\"toolbar-class\"\r\n          toolbarCustomButtons={[<FirstDropdownOption column={columns} />, <SecondDropdownOption agg={agg} />]}\r\n          placeholder={placeholder}\r\n          toolbar={{\r\n            options: ['inline', 'blockType', 'colorPicker'],\r\n            inline: {\r\n              options: ['bold', 'italic', 'underline'],\r\n              bold: { className: 'bordered-option-classname' },\r\n              italic: { className: 'bordered-option-classname' },\r\n              underline: { className: 'bordered-option-classname' },\r\n            },\r\n            blockType: {\r\n              inDropdown: true,\r\n              maxHeight: \"100px\", overflowY: \"auto\", columnCount: 2\r\n            },\r\n            colorPicker: {\r\n              component: undefined,\r\n              popupClassName: undefined,\r\n              colors: ['rgb(0, 0, 0)',\r\n                'rgb(255, 0, 0)',   // Red\r\n                'rgb(0, 255, 0)',   // Green\r\n                'rgb(0, 0, 255)',   // Blue\r\n                'rgb(255, 255, 0)', // Yellow\r\n                'rgb(255, 255, 255)']\r\n            }\r\n          }}\r\n        />\r\n        <Button editorState={editorState} />\r\n      </div>\r\n\r\n\r\n    );\r\n  }\r\n}\r\n\r\nexport default withStreamlitConnection(PandasTextEditor);",
         "import React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport PandasTextEditor from \"./PandasTextEditor\"\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <PandasTextEditor />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `st_pandas_text_editor-0.0.4/st_pandas_text_editor.egg-info/SOURCES.txt` & `st_pandas_text_editor-0.0.5/st_pandas_text_editor.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 st_pandas_text_editor/frontend/build/asset-manifest.json
 st_pandas_text_editor/frontend/build/bootstrap.min.css
 st_pandas_text_editor/frontend/build/index.html
 st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css
 st_pandas_text_editor/frontend/build/static/css/2.9b7094a5.chunk.css.map
 st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css
 st_pandas_text_editor/frontend/build/static/css/main.c21eaae6.chunk.css.map
-st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js
-st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.LICENSE.txt
-st_pandas_text_editor/frontend/build/static/js/2.ecfcc7a3.chunk.js.map
-st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js
-st_pandas_text_editor/frontend/build/static/js/main.baa131a3.chunk.js.map
+st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js
+st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.LICENSE.txt
+st_pandas_text_editor/frontend/build/static/js/2.817968fe.chunk.js.map
+st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js
+st_pandas_text_editor/frontend/build/static/js/main.7e37a4e5.chunk.js.map
 st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js
 st_pandas_text_editor/frontend/build/static/js/runtime-main.624f085e.js.map
```
