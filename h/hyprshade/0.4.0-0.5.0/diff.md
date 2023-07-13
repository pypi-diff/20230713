# Comparing `tmp/hyprshade-0.4.0.tar.gz` & `tmp/hyprshade-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.4.0.tar", max compression
+gzip compressed data, was "hyprshade-0.5.0.tar", max compression
```

## Comparing `hyprshade-0.4.0.tar` & `hyprshade-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.4.0/LICENSE
--rw-r--r--   0        0        0     2266 2023-07-13 03:26:40.709879 hyprshade-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.4.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.4.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2740 2023-07-13 13:17:34.751788 hyprshade-0.4.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.4.0/hyprshade/config.py
--rw-r--r--   0        0        0      524 2023-07-13 13:02:51.672749 hyprshade-0.4.0/hyprshade/constants.py
--rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.4.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.4.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1024 2023-07-13 13:18:06.239790 hyprshade-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.4.0/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.4.0/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 hyprshade-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 02:30:01.812307 hyprshade-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2266 2023-07-13 03:26:40.709879 hyprshade-0.5.0/README.md
+-rw-r--r--   0        0        0      125 2023-07-10 08:25:37.637388 hyprshade-0.5.0/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-12 10:22:13.964753 hyprshade-0.5.0/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-06 22:07:23.486991 hyprshade-0.5.0/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2740 2023-07-13 13:17:34.751788 hyprshade-0.5.0/hyprshade/cli.py
+-rw-r--r--   0        0        0     3718 2023-07-12 13:25:08.051277 hyprshade-0.5.0/hyprshade/config.py
+-rw-r--r--   0        0        0      524 2023-07-13 13:02:51.672749 hyprshade-0.5.0/hyprshade/constants.py
+-rw-r--r--   0        0        0      652 2023-07-13 13:07:02.148760 hyprshade-0.5.0/hyprshade/helpers.py
+-rw-r--r--   0        0        0      812 2023-07-12 12:09:47.053061 hyprshade-0.5.0/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-13 13:25:04.682808 hyprshade-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-12 02:45:17.153390 hyprshade-0.5.0/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-12 02:45:58.561385 hyprshade-0.5.0/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 hyprshade-0.5.0/PKG-INFO
```

### Comparing `hyprshade-0.4.0/LICENSE` & `hyprshade-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/README.md` & `hyprshade-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/hyprshade/cli.py` & `hyprshade-0.5.0/hyprshade/cli.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/hyprshade/config.py` & `hyprshade-0.5.0/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/hyprshade/constants.py` & `hyprshade-0.5.0/hyprshade/constants.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/hyprshade/helpers.py` & `hyprshade-0.5.0/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/hyprshade/utils.py` & `hyprshade-0.5.0/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/pyproject.toml` & `hyprshade-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
-include = ["shaders"]
+include = ["examples", "shaders"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = { extras = ["all"], version = "^0.9.0" }
 more-itertools = "^9.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `hyprshade-0.4.0/shaders/blue-light-filter.glsl` & `hyprshade-0.5.0/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/shaders/vibrance.glsl` & `hyprshade-0.5.0/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.4.0/PKG-INFO` & `hyprshade-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

