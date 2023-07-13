# Comparing `tmp/mkdocs_pages_j2_plugin-0.1.2.tar.gz` & `tmp/mkdocs_pages_j2_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pages_j2_plugin-0.1.2.tar", max compression
+gzip compressed data, was "mkdocs_pages_j2_plugin-0.2.0.tar", max compression
```

## Comparing `mkdocs_pages_j2_plugin-0.1.2.tar` & `mkdocs_pages_j2_plugin-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      867 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pagesj2/__init__.py
--rw-r--r--   0        0        0     2376 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pagesj2/plugin.py
--rw-r--r--   0        0        0     1256 2023-07-12 13:45:49.713079 mkdocs_pages_j2_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-07-13 20:43:55.914119 mkdocs_pages_j2_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 20:43:55.914119 mkdocs_pages_j2_plugin-0.2.0/pagesj2/__init__.py
+-rw-r--r--   0        0        0     2353 2023-07-13 20:43:55.914119 mkdocs_pages_j2_plugin-0.2.0/pagesj2/plugin.py
+-rw-r--r--   0        0        0     1256 2023-07-13 20:43:55.914119 mkdocs_pages_j2_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.2.0/PKG-INFO
```

### Comparing `mkdocs_pages_j2_plugin-0.1.2/README.md` & `mkdocs_pages_j2_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_pages_j2_plugin-0.1.2/pagesj2/plugin.py` & `mkdocs_pages_j2_plugin-0.2.0/pagesj2/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 loader=jinja2.FileSystemLoader(root),
             )
             for name in files:
                 if name != "pages.j2":
                     continue
 
                 template = env.get_template(name)
-                content = template.render(config=config, env=os.environ)
+                content = template.render(config)
                 dst = os.path.join(root, ".pages")
                 # Do not write the file if the content is the same.
                 # Otherwise, the "watcher" will continuously reload the page.
                 if os.path.exists(dst):
                     with open(
                         dst, encoding="utf-8"
                     ) as f:  # pylint: disable=invalid-name
```

### Comparing `mkdocs_pages_j2_plugin-0.1.2/pyproject.toml` & `mkdocs_pages_j2_plugin-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-pages-j2-plugin"
-version = "0.1.2"
+version = "0.2.0"
 description = "An MkDocs plugin to generate '.pages' from 'pages.j2'"
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-pages-j2-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "pagesj2" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
```

### Comparing `mkdocs_pages_j2_plugin-0.1.2/PKG-INFO` & `mkdocs_pages_j2_plugin-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-pages-j2-plugin
-Version: 0.1.2
+Version: 0.2.0
 Summary: An MkDocs plugin to generate '.pages' from 'pages.j2'
 Home-page: https://github.com/supcik/mkdocs-pages-j2-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
```

