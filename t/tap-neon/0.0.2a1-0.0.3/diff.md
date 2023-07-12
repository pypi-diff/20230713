# Comparing `tmp/tap_neon-0.0.2a1.tar.gz` & `tmp/tap_neon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_neon-0.0.2a1.tar", max compression
+gzip compressed data, was "tap_neon-0.0.3.tar", max compression
```

## Comparing `tap_neon-0.0.2a1.tar` & `tap_neon-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2631 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/README.md
--rw-r--r--   0        0        0     1817 2023-06-06 16:20:12.789329 tap_neon-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__init__.py
--rw-r--r--   0        0        0      107 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/__main__.py
--rw-r--r--   0        0        0     2593 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/client.py
--rw-r--r--   0        0        0     2931 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/streams.py
--rw-r--r--   0        0        0     2905 2023-06-06 16:19:55.029003 tap_neon-0.0.2a1/tap_neon/tap.py
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 tap_neon-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     2631 2023-07-12 23:27:58.701577 tap_neon-0.0.3/README.md
+-rw-r--r--   0        0        0     1815 2023-07-12 23:28:15.361608 tap_neon-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/__init__.py
+-rw-r--r--   0        0        0      107 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/__main__.py
+-rw-r--r--   0        0        0     2593 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/client.py
+-rw-r--r--   0        0        0     3543 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/streams.py
+-rw-r--r--   0        0        0     2905 2023-07-12 23:27:58.701577 tap_neon-0.0.3/tap_neon/tap.py
+-rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 tap_neon-0.0.3/PKG-INFO
```

### Comparing `tap_neon-0.0.2a1/README.md` & `tap_neon-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2a1/pyproject.toml` & `tap_neon-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,55 @@
 requires = [
   "poetry-core<2,>=1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-neon"
-version = "0.0.2a1"
+version = "0.0.3"
 description = "`tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramirez <edgarrm358@gmail.com>"]
 keywords = ["ELT", "singer.io", "Neon Serverless Postgres"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-neon"
 repository = "https://github.com/edgarrmondragon/tap-neon"
 documentation = "https://github.com/edgarrmondragon/tap-neon#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.28.0"
+singer-sdk = "0.30.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.1"
 
 [tool.poetry.scripts]
 # CLI declaration
 "tap-neon" = "tap_neon.tap:TapNeon.cli"
 
+[tool.ruff]
+ignore = ["ANN101", "DJ", "PD"]
+line-length = 88
+select = ["ALL"]
+src = ["tap_neon"]
+
+[tool.ruff.flake8-annotations]
+allow-star-arg-any = true
+
+[tool.ruff.isort]
+known-first-party = ["tap_neon"]
+required-imports = ["from __future__ import annotations"]
+
+[tool.ruff.per-file-ignores]
+"noxfile.py" = ["ANN"]
+"tests/*" = ["ANN"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.pytest.ini_options]
 addopts = "-vvv"
 
 [tool.mypy]
 python_version = "3.10"
 warn_unused_configs = true
 
@@ -45,27 +65,7 @@
     {%- else -%}
         {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
     {%- endif -%}
 """
 metadata = true
 style = "pep440"
 vcs = "git"
-
-[tool.ruff]
-ignore = ["ANN101", "DJ", "PD"]
-line-length = 88
-select = ["ALL"]
-src = ["tap_neon"]
-
-[tool.ruff.flake8-annotations]
-allow-star-arg-any = true
-
-[tool.ruff.isort]
-known-first-party = ["tap_neon"]
-required-imports = ["from __future__ import annotations"]
-
-[tool.ruff.per-file-ignores]
-"noxfile.py" = ["ANN"]
-"tests/*" = ["ANN"]
-
-[tool.ruff.pydocstyle]
-convention = "google"
```

### Comparing `tap_neon-0.0.2a1/tap_neon/client.py` & `tap_neon-0.0.3/tap_neon/client.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2a1/tap_neon/tap.py` & `tap_neon-0.0.3/tap_neon/tap.py`

 * *Files identical despite different names*

### Comparing `tap_neon-0.0.2a1/PKG-INFO` & `tap_neon-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-neon
-Version: 0.0.2a1
+Version: 0.0.3
 Summary: `tap-neon` is a Singer tap for Neon Serverless Postgres, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-neon
 License: Apache 2.0
 Keywords: ELT,singer.io,Neon Serverless Postgres
 Author: Edgar Ramirez
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.28.0)
+Requires-Dist: singer-sdk (==0.30.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-neon#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-neon
 Description-Content-Type: text/markdown
 
 # `tap-neon`
 
 Singer tap for Neon Serverless Postgres.
```

