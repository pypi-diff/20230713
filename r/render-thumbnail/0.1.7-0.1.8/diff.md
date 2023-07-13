# Comparing `tmp/render_thumbnail-0.1.7.tar.gz` & `tmp/render_thumbnail-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_thumbnail-0.1.7.tar", max compression
+gzip compressed data, was "render_thumbnail-0.1.8.tar", max compression
```

## Comparing `render_thumbnail-0.1.7.tar` & `render_thumbnail-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.7/README.md
--rw-r--r--   0        0        0      401 2023-07-13 17:58:04.124450 render_thumbnail-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.7/render_thumbnail/__init__.py
--rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.7/render_thumbnail/__main__.py
--rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.7/render_thumbnail/functions_tex.py
--rw-r--r--   0        0        0     2659 2023-07-13 17:57:51.685734 render_thumbnail-0.1.7/render_thumbnail/main.py
--rw-r--r--   0        0        0      304 1970-01-01 00:00:00.000000 render_thumbnail-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147713 render_thumbnail-0.1.8/README.md
+-rw-r--r--   0        0        0      401 2023-07-13 18:01:34.321969 render_thumbnail-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 16:03:38.147641 render_thumbnail-0.1.8/render_thumbnail/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-13 08:35:52.973584 render_thumbnail-0.1.8/render_thumbnail/__main__.py
+-rw-r--r--   0        0        0     2170 2023-07-12 16:06:45.557696 render_thumbnail-0.1.8/render_thumbnail/functions_tex.py
+-rw-r--r--   0        0        0     2656 2023-07-13 18:01:25.938702 render_thumbnail-0.1.8/render_thumbnail/main.py
+-rw-r--r--   0        0        0      304 1970-01-01 00:00:00.000000 render_thumbnail-0.1.8/PKG-INFO
```

### Comparing `render_thumbnail-0.1.7/render_thumbnail/functions_tex.py` & `render_thumbnail-0.1.8/render_thumbnail/functions_tex.py`

 * *Files identical despite different names*

### Comparing `render_thumbnail-0.1.7/render_thumbnail/main.py` & `render_thumbnail-0.1.8/render_thumbnail/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         file.write(f'\\end{{document}}')
 
 
 
     try:
         print(os.getcwd)
-        os.chdir("cd ./thumbnail")
+        os.chdir("./thumbnail")
         try:
             os.system("pdflatex -shell-escape main.tex")
         except:
             click.echo("Failed to rum pdflatex")
     except:
         click.echo("Failed to run cddir")
```

