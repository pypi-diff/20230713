# Comparing `tmp/render_thumbnail-0.1.0.tar.gz` & `tmp/render_thumbnail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_thumbnail-0.1.0.tar", max compression
+gzip compressed data, was "render_thumbnail-0.1.1.tar", max compression
```

## Comparing `render_thumbnail-0.1.0.tar` & `render_thumbnail-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.0/README.md
--rw-r--r--   0        0        0      691 2023-07-13 08:41:11.304145 render_thumbnail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.0/render_thumbnail/__init__.py
--rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.0/render_thumbnail/__main__.py
--rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.0/render_thumbnail/functions_tex.py
--rw-r--r--   0        0        0     2519 2023-07-13 17:23:26.262748 render_thumbnail-0.1.0/render_thumbnail/main.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 render_thumbnail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.1/README.md
+-rw-r--r--   0        0        0      691 2023-07-13 17:30:21.586967 render_thumbnail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.1/render_thumbnail/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.1/render_thumbnail/__main__.py
+-rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.1/render_thumbnail/functions_tex.py
+-rw-r--r--   0        0        0     2566 2023-07-13 17:30:09.747676 render_thumbnail-0.1.1/render_thumbnail/main.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 render_thumbnail-0.1.1/PKG-INFO
```

### Comparing `render_thumbnail-0.1.0/pyproject.toml` & `render_thumbnail-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "render-thumbnail"
-version = "0.1.0"
+version = "0.1.1"
 description = "A CLI tool written in python using click package for creating thumbnail for youtube using the tex file it basically extracts tikzpicture environment from the tex file and put it into separate tex file and then it renders as pdf then to manually you can export as png usign vbpdf instagram tool."
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "render_thumbnail"}]
 
 
 [tool.poetry.scripts]
```

### Comparing `render_thumbnail-0.1.0/render_thumbnail/functions_tex.py` & `render_thumbnail-0.1.1/render_thumbnail/functions_tex.py`

 * *Files identical despite different names*

### Comparing `render_thumbnail-0.1.0/render_thumbnail/main.py` & `render_thumbnail-0.1.1/render_thumbnail/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             file.write(f'{tikz_render.replace("tikz.tex", files[nthtikz - 1])}\n')
 
         file.write(f'\\end{{document}}')
 
 
 
     try:
+        os.system(f'cd {path_tikz}/thumbnail')
         os.system(f'pdflatex -shell-escape {path_main}')
     except:
         click.echo("Failed to run pdflatex")
```

### Comparing `render_thumbnail-0.1.0/PKG-INFO` & `render_thumbnail-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-thumbnail
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI tool written in python using click package for creating thumbnail for youtube using the tex file it basically extracts tikzpicture environment from the tex file and put it into separate tex file and then it renders as pdf then to manually you can export as png usign vbpdf instagram tool.
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

