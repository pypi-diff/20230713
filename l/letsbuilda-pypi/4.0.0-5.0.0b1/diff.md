# Comparing `tmp/letsbuilda-pypi-4.0.0.tar.gz` & `tmp/letsbuilda-pypi-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-4.0.0.tar", last modified: Wed Apr 26 02:39:53 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-5.0.0b1.tar", last modified: Thu Jul 13 05:09:48 2023, max compression
```

## Comparing `letsbuilda-pypi-4.0.0.tar` & `letsbuilda-pypi-5.0.0b1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/src/letsbuilda/pypi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 02:39:53.000000 letsbuilda-pypi-4.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:39:53.276563 letsbuilda-pypi-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-26 02:39:44.000000 letsbuilda-pypi-4.0.0/tests/test_rss_feed_parsing.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-07-12 21:27:21.000000 letsbuilda-pypi-5.0.0b1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      644 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1264 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.344054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2435 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/async_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      880 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/files.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3572 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_json.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1383 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_package.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1200 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_rss.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2121 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/sync_client.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      146 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/tests/test_rss_feed_parsing.py
```

### Comparing `letsbuilda-pypi-4.0.0/LICENSE` & `letsbuilda-pypi-5.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-4.0.0/pyproject.toml` & `letsbuilda-pypi-5.0.0b1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 [project]
 name = "letsbuilda-pypi"
-version = "4.0.0"
+version = "5.0.0b1"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11.4"
 dependencies = [
-    "aiohttp",
+    "requests",
     "xmltodict",
-    "pendulum",
 ]
 
 [project.urls]
 repository = "https://github.com/letsbuilda/letsbuilda-pypi/"
 documentation = "https://docs.letsbuilda.dev/letsbuilda-pypi/"
 
 [project.optional-dependencies]
+async = [
+    "aiohttp",
+]
 dev = [
+    "pre-commit",
     "black",
-    "isort",
     "ruff",
 ]
 tests = [
     "pytest",
+
+    # from async extra
+    "aiohttp",
 ]
 docs = [
     "sphinx",
     "furo",
     "sphinx-autoapi",
     "releases",
     "toml",
+
+    # from async extra
+    "aiohttp",
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[tool.sphinx]
-copyright = "Let's build a ..."
-author = "Bradley Reynolds"
-
-[tool.isort]
-profile = "black"
-
 [tool.black]
-target-version = ["py310"]
+target-version = ["py311"]
 line-length = 120
 
 [tool.ruff]
+select = ["ALL"]
+ignore = [
+  "PLC0414", # (Import alias does not rename original package) - Re-exporting
+]
+target-version = "py311"
 line-length = 120
 
+[tool.ruff.isort]
+known-first-party = ["letsbuilda.pypi"]
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
+
 [tool.pytest.ini_options]
 addopts = "tests -r a -v --doctest-modules src"
```

