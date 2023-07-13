# Comparing `tmp/render_thumbnail-0.1.4.tar.gz` & `tmp/render_thumbnail-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_thumbnail-0.1.4.tar", max compression
+gzip compressed data, was "render_thumbnail-0.1.5.tar", max compression
```

## Comparing `render_thumbnail-0.1.4.tar` & `render_thumbnail-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.4/README.md
--rw-r--r--   0        0        0      420 2023-07-13 17:46:08.006085 render_thumbnail-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.4/render_thumbnail/__init__.py
--rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.4/render_thumbnail/__main__.py
--rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.4/render_thumbnail/functions_tex.py
--rw-r--r--   0        0        0     2567 2023-07-13 17:45:42.904674 render_thumbnail-0.1.4/render_thumbnail/main.py
--rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 render_thumbnail-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.5/README.md
+-rw-r--r--   0        0        0      455 2023-07-13 17:52:04.665851 render_thumbnail-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.5/render_thumbnail/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.5/render_thumbnail/__main__.py
+-rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.5/render_thumbnail/functions_tex.py
+-rw-r--r--   0        0        0     2582 2023-07-13 17:51:19.815637 render_thumbnail-0.1.5/render_thumbnail/main.py
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 render_thumbnail-0.1.5/PKG-INFO
```

### Comparing `render_thumbnail-0.1.4/render_thumbnail/functions_tex.py` & `render_thumbnail-0.1.5/render_thumbnail/functions_tex.py`

 * *Files identical despite different names*

### Comparing `render_thumbnail-0.1.4/render_thumbnail/main.py` & `render_thumbnail-0.1.5/render_thumbnail/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,16 @@
             file.write(f'{tikz_render.replace("tikz.tex", files[nthtikz - 1])}\n')
 
         file.write(f'\\end{{document}}')
 
 
 
     try:
-        os.chdir(f'cd {path_tikz}/thumbnail')
+        os.chdir(f'cd ./thumbnail')
+        print(os.getcwd)
         os.system(f'pdflatex -shell-escape main.tex')
     except:
         click.echo("Failed to run pdflatex")
```

