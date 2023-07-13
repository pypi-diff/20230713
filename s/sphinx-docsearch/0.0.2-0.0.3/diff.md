# Comparing `tmp/sphinx_docsearch-0.0.2.tar.gz` & `tmp/sphinx_docsearch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_docsearch-0.0.2.tar", max compression
+gzip compressed data, was "sphinx_docsearch-0.0.3.tar", max compression
```

## Comparing `sphinx_docsearch-0.0.2.tar` & `sphinx_docsearch-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-07-13 07:20:47.601023 sphinx_docsearch-0.0.2/LICENSE
--rw-r--r--   0        0        0     1062 2023-07-13 07:20:47.601023 sphinx_docsearch-0.0.2/README.md
--rw-r--r--   0        0        0     1672 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4737 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/py.typed
--rw-r--r--   0        0        0      130 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
--rw-r--r--   0        0        0    13261 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.css
--rw-r--r--   0        0        0   126677 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.js
--rw-r--r--   0        0        0      648 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch_config.js_t
--rw-r--r--   0        0        0      416 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/furo-docsearch-custom.css
--rw-r--r--   0        0        0      167 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/rtd-docsearch-custom.css
--rw-r--r--   0        0        0      117 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/templates/searchbox.html
--rw-r--r--   0        0        0      117 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/templates/sidebar/search.html
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1579 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/README.md
+-rw-r--r--   0        0        0     1672 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4968 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/py.typed
+-rw-r--r--   0        0        0      130 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
+-rw-r--r--   0        0        0    13261 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch.css
+-rw-r--r--   0        0        0   126677 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch.js
+-rw-r--r--   0        0        0      648 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch_config.js_t
+-rw-r--r--   0        0        0     1782 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/furo-docsearch-custom.css
+-rw-r--r--   0        0        0      167 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/rtd-docsearch-custom.css
+-rw-r--r--   0        0        0      117 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/templates/searchbox.html
+-rw-r--r--   0        0        0      117 2023-07-13 08:55:29.533633 sphinx_docsearch-0.0.3/src/sphinx_docsearch/templates/sidebar/search.html
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.3/PKG-INFO
```

### Comparing `sphinx_docsearch-0.0.2/LICENSE` & `sphinx_docsearch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.2/pyproject.toml` & `sphinx_docsearch-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-docsearch"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Sphinx extension for replacing the built-in search with Algolia DocSearch"
 authors = ["Algolia"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "sphinx_docsearch", from = "src"}
 ]
@@ -25,15 +25,15 @@
 ruff = "*"
 black = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = "^2021.3.14"
 python-dotenv = "^1.0.0"
 furo = "^2023.5.20"
-myst-parser = "^1.0.0"
+myst-parser = "^2.0.0"
 sphinx_rtd_theme = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 beautifulsoup4 = "^4.12.2"
 pytest-cov = "^4.0.0"
 mypy = "^1.2.0"
```

### Comparing `sphinx_docsearch-0.0.2/src/sphinx_docsearch/__init__.py` & `sphinx_docsearch-0.0.3/src/sphinx_docsearch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,31 +43,35 @@
         logger.warning(
             __("You must provide your Algolia index name for DocSearch to work.")
         )
 
 
 @progress_message("DocSearch: set up")
 def add_docsearch_assets(app: Sphinx, config: Config) -> None:
-    """Add the CSS and JS files for DocSearch."""
-    app.add_css_file("docsearch.css")
+    """Add the CSS and JS files for DocSearch.
+
+    Load the CSS with priority 800 to make sure it's loaded after default CSS.
+    This prevents global CSS (often used in Sphinx themes) from overriding DocSearch CSS.
+    """
+    app.add_css_file("docsearch.css", priority=800)
     app.add_js_file("docsearch.js", loading_method="defer")
     app.add_js_file("docsearch_config.js", loading_method="defer")
 
     static_path = Path(__file__).parent.joinpath("static").absolute()
     templates_path = Path(__file__).parent.joinpath("templates").absolute()
     config.html_static_path.append(str(static_path))
     config.templates_path.append(str(templates_path))
 
     # Provide custom CSS to support different themes
     if config.html_theme == "furo":
-        app.add_css_file("furo-docsearch-custom.css")
+        app.add_css_file("furo-docsearch-custom.css", priority=810)
     elif config.html_theme == "sphinx_rtd_theme":
-        app.add_css_file("rtd-docsearch-custom.css")
+        app.add_css_file("rtd-docsearch-custom.css", priority=820)
     elif config.html_theme == "alabaster":
-        app.add_css_file("alabaster-docsearch-custom.css")
+        app.add_css_file("alabaster-docsearch-custom.css", priority=820)
 
 
 @progress_message("DocSearch: update global context")
 def update_global_context(app: Sphinx, doctree: Node, docname: str) -> None:
     """Update global context with DocSearch configuration."""
     if app.builder.format != "html":
         return
```

### Comparing `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.css` & `sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.js` & `sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch.js`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch_config.js_t` & `sphinx_docsearch-0.0.3/src/sphinx_docsearch/static/docsearch_config.js_t`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.2/PKG-INFO` & `sphinx_docsearch-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-docsearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Sphinx extension for replacing the built-in search with Algolia DocSearch
 License: MIT
 Author: Algolia
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
@@ -16,50 +16,57 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: sphinx (>=6.2.1,<7.0.0)
 Description-Content-Type: text/markdown
 
-# Algolia DocSearch Sphinx extension
+# Algolia DocSearch for Sphinx
 
 This extension for the [Sphinx](https://www.sphinx-doc.org/en/master/) documentation generator
 replaces Sphinx's built-in search with Algolia DocSearch.
 
 ## Before you begin
 
-[**Apply for DocSearch**](https://docsearch.algolia.com/apply). You'll get an email with your Algolia credentials.
+[**Apply for DocSearch**](https://docsearch.algolia.com/apply).
+You'll get an email with your Algolia credentials.
 
 This extension supports Python versions 3.8, 3.9, 3.10, and 3.11 and Sphinx versions 5 and later.
 
 ## Install
 
-Install the `sphinx-docsearch` extension from PyPI:
+Install the `sphinx-docsearch` package:
 
 ```sh
 pip install sphinx-docsearch
 ```
 
 ## Configure
 
-1. Add `sphinx-docsearch` to your Sphinx configuration file `conf.py`:
+1. Add `sphinx-docsearch` to your Sphinx configuration:
 
    ```python
+   # conf.py
    extensions += ["sphinx_docsearch"]
    ```
 
 1. Add your Algolia credentials to your Sphinx configuration:
 
    ```python
+   # conf.py
    docsearch_app_id = "<DOCSEARCH_APP_ID>"
    docsearch_api_key = "<DOCSEARCH_SEARCH_API_KEY>"
    docsearch_index_name = "<DOCSEARCH_INDEX_NAME>"
    ```
 
-1. Optional: change configuration settings
+   See also: [Configure DocSearch](https://sphinx-docsearch.readthedocs.io/en/latest/configuration.html).
 
 ## Customize
 
-- Customize crawling (link to DocSearch or Crawler doc)
-- Add custom templates
-- Add custom CSS
+To change what the crawler should extract from your pages, see [Record Extractor](https://docsearch.algolia.com/docs/record-extractor).
+
+You can add [custom templates](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-templates),
+if your Sphinx HTML theme uses templates [not provided](https://sphinx-docsearch.readthedocs.io/en/latest/themes.html)
+by this extension.
+
+You can customize the look of the DocSearch UI by [adding your own CSS](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-css).
```

