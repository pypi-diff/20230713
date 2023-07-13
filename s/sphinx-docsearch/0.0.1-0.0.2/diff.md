# Comparing `tmp/sphinx_docsearch-0.0.1.tar.gz` & `tmp/sphinx_docsearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_docsearch-0.0.1.tar", max compression
+gzip compressed data, was "sphinx_docsearch-0.0.2.tar", max compression
```

## Comparing `sphinx_docsearch-0.0.1.tar` & `sphinx_docsearch-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/LICENSE
--rw-r--r--   0        0        0     1061 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/README.md
--rw-r--r--   0        0        0     1672 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4737 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/py.typed
--rw-r--r--   0        0        0      130 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
--rw-r--r--   0        0        0    13261 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch.css
--rw-r--r--   0        0        0   126677 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch.js
--rw-r--r--   0        0        0      648 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch_config.js_t
--rw-r--r--   0        0        0      473 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/furo-docsearch-custom.css
--rw-r--r--   0        0        0      167 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/rtd-docsearch-custom.css
--rw-r--r--   0        0        0      117 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/templates/searchbox.html
--rw-r--r--   0        0        0      117 2023-07-12 13:26:41.207398 sphinx_docsearch-0.0.1/src/sphinx_docsearch/templates/sidebar/search.html
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 07:20:47.601023 sphinx_docsearch-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1062 2023-07-13 07:20:47.601023 sphinx_docsearch-0.0.2/README.md
+-rw-r--r--   0        0        0     1672 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4737 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/py.typed
+-rw-r--r--   0        0        0      130 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
+-rw-r--r--   0        0        0    13261 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.css
+-rw-r--r--   0        0        0   126677 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.js
+-rw-r--r--   0        0        0      648 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch_config.js_t
+-rw-r--r--   0        0        0      416 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/furo-docsearch-custom.css
+-rw-r--r--   0        0        0      167 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/rtd-docsearch-custom.css
+-rw-r--r--   0        0        0      117 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/templates/searchbox.html
+-rw-r--r--   0        0        0      117 2023-07-13 07:20:47.605023 sphinx_docsearch-0.0.2/src/sphinx_docsearch/templates/sidebar/search.html
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.2/PKG-INFO
```

### Comparing `sphinx_docsearch-0.0.1/LICENSE` & `sphinx_docsearch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.1/README.md` & `sphinx_docsearch-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 ## Configure
 
 1. Add `sphinx-docsearch` to your Sphinx configuration file `conf.py`:
 
    ```python
-   extensions += ["sphinx_docsearch]
+   extensions += ["sphinx_docsearch"]
    ```
 
 1. Add your Algolia credentials to your Sphinx configuration:
 
    ```python
    docsearch_app_id = "<DOCSEARCH_APP_ID>"
    docsearch_api_key = "<DOCSEARCH_SEARCH_API_KEY>"
```

### Comparing `sphinx_docsearch-0.0.1/pyproject.toml` & `sphinx_docsearch-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-docsearch"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Sphinx extension for replacing the built-in search with Algolia DocSearch"
 authors = ["Algolia"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "sphinx_docsearch", from = "src"}
 ]
```

### Comparing `sphinx_docsearch-0.0.1/src/sphinx_docsearch/__init__.py` & `sphinx_docsearch-0.0.2/src/sphinx_docsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch.css` & `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch.js` & `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch.js`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.1/src/sphinx_docsearch/static/docsearch_config.js_t` & `sphinx_docsearch-0.0.2/src/sphinx_docsearch/static/docsearch_config.js_t`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.1/PKG-INFO` & `sphinx_docsearch-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-docsearch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Sphinx extension for replacing the built-in search with Algolia DocSearch
 License: MIT
 Author: Algolia
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 ```
 
 ## Configure
 
 1. Add `sphinx-docsearch` to your Sphinx configuration file `conf.py`:
 
    ```python
-   extensions += ["sphinx_docsearch]
+   extensions += ["sphinx_docsearch"]
    ```
 
 1. Add your Algolia credentials to your Sphinx configuration:
 
    ```python
    docsearch_app_id = "<DOCSEARCH_APP_ID>"
    docsearch_api_key = "<DOCSEARCH_SEARCH_API_KEY>"
```

