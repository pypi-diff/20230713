# Comparing `tmp/ctktablerowselector-1.0.0.tar.gz` & `tmp/ctktablerowselector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctktablerowselector-1.0.0.tar", max compression
+gzip compressed data, was "ctktablerowselector-1.0.1.tar", max compression
```

## Comparing `ctktablerowselector-1.0.0.tar` & `ctktablerowselector-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6508 2023-07-13 12:01:39.896659 ctktablerowselector-1.0.0/CTkTableRowSelector/__init__.py
--rw-r--r--   0        0        0     1656 2023-07-13 00:26:44.966115 ctktablerowselector-1.0.0/CTkTableRowSelector/__main__.py
--rw-r--r--   0        0        0     1493 2023-07-13 13:06:08.987918 ctktablerowselector-1.0.0/README.md
--rw-r--r--   0        0        0      741 2023-07-13 13:33:55.746628 ctktablerowselector-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 ctktablerowselector-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6508 2023-07-13 12:01:39.896659 ctktablerowselector-1.0.1/CTkTableRowSelector/__init__.py
+-rw-r--r--   0        0        0     1656 2023-07-13 00:26:44.966115 ctktablerowselector-1.0.1/CTkTableRowSelector/__main__.py
+-rw-r--r--   0        0        0     1480 2023-07-13 13:46:23.050962 ctktablerowselector-1.0.1/README.md
+-rw-r--r--   0        0        0      810 2023-07-13 13:53:35.485952 ctktablerowselector-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 ctktablerowselector-1.0.1/PKG-INFO
```

### Comparing `ctktablerowselector-1.0.0/CTkTableRowSelector/__init__.py` & `ctktablerowselector-1.0.1/CTkTableRowSelector/__init__.py`

 * *Files identical despite different names*

### Comparing `ctktablerowselector-1.0.0/CTkTableRowSelector/__main__.py` & `ctktablerowselector-1.0.1/CTkTableRowSelector/__main__.py`

 * *Files identical despite different names*

### Comparing `ctktablerowselector-1.0.0/README.md` & `ctktablerowselector-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,24 @@
+Metadata-Version: 2.1
+Name: ctktablerowselector
+Version: 1.0.1
+Summary: Wrapper class around CTkTable to let users select rows
+Home-page: https://github.com/CallMePixelMan/CTkTableRowSelector
+License: MIT
+Author: CallMePixelMan
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ctktable (>=0.7,<0.8)
+Project-URL: Repository, https://github.com/CallMePixelMan/CTkTableRowSelector
+Description-Content-Type: text/markdown
+
 # CTkTableRowSelector
-A small and stable extension above CTkTable to let users select rows.
+Wrapper class around CTkTable to let users select rows.
 ![PyPI](https://img.shields.io/pypi/v/ctktablerowselector)
 ![PyPI - License](https://img.shields.io/pypi/l/ctktablerowselector)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Features
 - [x] Plug&Play: No shady attributes, create an instance and get the values you need.
 - [x] Easy to use interface.
@@ -45,8 +60,9 @@
 )
 button.pack(pady=(0, 20))
 
 root.mainloop()
 ```
 
 ## Licence
-This project is delivered under the MIT Licence.
+This project is delivered under the MIT Licence.
+
```

### Comparing `ctktablerowselector-1.0.0/pyproject.toml` & `ctktablerowselector-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "CTkTableRowSelector"
-version = "1.0.0"
+version = "1.0.1"
 description = "Wrapper class around CTkTable to let users select rows"
 authors = ["CallMePixelMan"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/CallMePixelMan/CTkTableRowSelector"
 packages = [
     { include = "CTkTableRowSelector" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 ctktable = "^0.7"
```

