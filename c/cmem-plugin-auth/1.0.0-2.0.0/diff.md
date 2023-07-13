# Comparing `tmp/cmem-plugin-auth-1.0.0.tar.gz` & `tmp/cmem_plugin_auth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem-plugin-auth-1.0.0.tar", max compression
+gzip compressed data, was "cmem_plugin_auth-2.0.0.tar", max compression
```

## Comparing `cmem-plugin-auth-1.0.0.tar` & `cmem_plugin_auth-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11334 2022-10-12 11:13:44.770092 cmem-plugin-auth-1.0.0/LICENSE
--rw-r--r--   0        0        0      369 2022-10-12 11:13:49.891715 cmem-plugin-auth-1.0.0/README-public.md
--rw-r--r--   0        0        0        0 2022-10-12 11:13:41.263373 cmem-plugin-auth-1.0.0/cmem_plugin_auth/__init__.py
--rw-r--r--   0        0        0        0 2022-10-12 11:13:50.785682 cmem-plugin-auth-1.0.0/cmem_plugin_auth/workflow/__init__.py
--rw-r--r--   0        0        0     6638 2022-10-12 15:26:58.304056 cmem-plugin-auth-1.0.0/cmem_plugin_auth/workflow/auth.py
--rw-r--r--   0        0        0     1537 2022-10-12 15:34:29.218196 cmem-plugin-auth-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 cmem-plugin-auth-1.0.0/setup.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 cmem-plugin-auth-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-13 00:20:57.154968 cmem_plugin_auth-2.0.0/LICENSE
+-rw-r--r--   0        0        0      369 2023-07-13 00:20:57.154968 cmem_plugin_auth-2.0.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-13 00:20:57.154968 cmem_plugin_auth-2.0.0/cmem_plugin_auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 00:20:57.154968 cmem_plugin_auth-2.0.0/cmem_plugin_auth/workflow/__init__.py
+-rw-r--r--   0        0        0     6638 2023-07-13 00:20:57.154968 cmem_plugin_auth-2.0.0/cmem_plugin_auth/workflow/auth.py
+-rw-r--r--   0        0        0     1664 2023-07-13 00:21:28.419328 cmem_plugin_auth-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 cmem_plugin_auth-2.0.0/PKG-INFO
```

### Comparing `cmem-plugin-auth-1.0.0/LICENSE` & `cmem_plugin_auth-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem-plugin-auth-1.0.0/cmem_plugin_auth/workflow/auth.py` & `cmem_plugin_auth-2.0.0/cmem_plugin_auth/workflow/auth.py`

 * *Files identical despite different names*

### Comparing `cmem-plugin-auth-1.0.0/pyproject.toml` & `cmem_plugin_auth-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [tool.poetry]
 name = "cmem-plugin-auth"
-version = "1.0.0"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "Authenticate to services and provide the OAuth2 access token for other tasks."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin"
 ]
+homepage = "https://github.com/eccenca/cmem-plugin-auth"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^2.1.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 requests-oauthlib = "^1.3.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^3.0.0"
-black = "^22.1.0"
-bandit = "^1.7.2"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^0.931"
-coverage = "^6.3.2"
-defusedxml = "^0.7.1"
+typed-ast = "^1.5.4"
+wheel = "^0.38.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `cmem-plugin-auth-1.0.0/PKG-INFO` & `cmem_plugin_auth-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-auth
-Version: 1.0.0
+Version: 2.0.0
 Summary: Authenticate to services and provide the OAuth2 access token for other tasks.
+Home-page: https://github.com/eccenca/cmem-plugin-auth
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=2.1.0,<3.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-auth
 
 Authenticate to services and provide the OAuth2 access token for other tasks.
```

