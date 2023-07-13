# Comparing `tmp/neuro_all-23.7.0.tar.gz` & `tmp/neuro_all-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro_all-23.7.0.tar", max compression
+gzip compressed data, was "neuro_all-23.7.1.tar", max compression
```

## Comparing `neuro_all-23.7.0.tar` & `neuro_all-23.7.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-06 23:26:30.096095 neuro_all-23.7.0/LICENSE
--rw-r--r--   0        0        0      107 2023-07-06 23:26:30.096095 neuro_all-23.7.0/README.md
--rw-r--r--   0        0        0      462 2023-07-06 23:26:30.100096 neuro_all-23.7.0/neuro_all/__init__.py
--rw-r--r--   0        0        0     1659 2023-07-06 23:26:30.100096 neuro_all-23.7.0/pyproject.toml
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 neuro_all-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 16:17:54.862367 neuro_all-23.7.1/LICENSE
+-rw-r--r--   0        0        0      107 2023-07-13 16:17:54.862367 neuro_all-23.7.1/README.md
+-rw-r--r--   0        0        0      462 2023-07-13 16:17:54.862367 neuro_all-23.7.1/neuro_all/__init__.py
+-rw-r--r--   0        0        0     1658 2023-07-13 16:17:54.866367 neuro_all-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 neuro_all-23.7.1/PKG-INFO
```

### Comparing `neuro_all-23.7.0/LICENSE` & `neuro_all-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro_all-23.7.0/pyproject.toml` & `neuro_all-23.7.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuro-all"
-version = "23.7.0"
+version = "23.7.1"
 description = "Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command"
 authors = ["Neu.ro Team <team@neu.ro>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://neu.ro"
 repository = "https://github.com/neuro-inc/neuro-all"
 keywords = [
@@ -40,19 +40,19 @@
 docker-credential-neuro = "neuro_cli.docker_credential_helper:main"
 neuro-extras = "neuro_extras:main"
 neuro-flow = "neuro_flow.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
 neuro-cli = "23.7.0"
-neuro-extras = "23.7.0"
+neuro-extras = "23.7.1"
 neuro-flow = "23.7.0"
 certifi = "2022.12.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "7.2.1"
-pre-commit = "^2.21.0"
-click = "^8.1.3"
+pytest = "7.4.0"
+pre-commit = "^3.3.3"
+click = "^8.1.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `neuro_all-23.7.0/PKG-INFO` & `neuro_all-23.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-all
-Version: 23.7.0
+Version: 23.7.1
 Summary: Combo package for installing all neu.ro command line tools by 'pipx install neuro-all' command
 Home-page: https://neu.ro
 License: Apache-2.0
 Keywords: neu.ro,mlops
 Author: Neu.ro Team
 Author-email: team@neu.ro
 Requires-Python: >=3.8.0,<4.0.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: neuro-cli (==23.7.0)
-Requires-Dist: neuro-extras (==23.7.0)
+Requires-Dist: neuro-extras (==23.7.1)
 Requires-Dist: neuro-flow (==23.7.0)
 Project-URL: Repository, https://github.com/neuro-inc/neuro-all
 Description-Content-Type: text/markdown
 
 # neuro-all
 Combo package for installing all neu.ro command line tools by `pipx install neuro-all` command
```

