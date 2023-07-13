# Comparing `tmp/odd_cli-0.1.8.tar.gz` & `tmp/odd_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_cli-0.1.8.tar", max compression
+gzip compressed data, was "odd_cli-0.1.9.tar", max compression
```

## Comparing `odd_cli-0.1.8.tar` & `odd_cli-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:05:09.000000 odd_cli-0.1.8/LICENSE
--rw-r--r--   0        0        0     2021 2023-02-09 17:05:09.000000 odd_cli-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/__init__.py
--rw-r--r--   0        0        0     1247 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/client.py
--rw-r--r--   0        0        0      150 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/error.py
--rw-r--r--   0        0        0      460 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/logger.py
--rw-r--r--   0        0        0     1093 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/main.py
--rw-r--r--   0        0        0        0 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/__init__.py
--rw-r--r--   0        0        0     1683 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/csv.py
--rw-r--r--   0        0        0        0 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/mapper/__init__.py
--rw-r--r--   0        0        0     1044 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/mapper/field.py
--rw-r--r--   0        0        0      733 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/mapper/table.py
--rw-r--r--   0        0        0        0 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/models/__init__.py
--rw-r--r--   0        0        0      599 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/models/field.py
--rw-r--r--   0        0        0      218 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/models/table.py
--rw-r--r--   0        0        0     1161 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/reader/reader.py
--rw-r--r--   0        0        0      747 2023-02-09 17:05:09.000000 odd_cli-0.1.8/odd_cli/tokens.py
--rw-r--r--   0        0        0      813 2023-02-09 17:05:29.000000 odd_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 odd_cli-0.1.8/setup.py
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 odd_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-14 08:40:43.000000 odd_cli-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2021 2023-02-14 08:40:43.000000 odd_cli-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/__init__.py
+-rw-r--r--   0        0        0     1247 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/client.py
+-rw-r--r--   0        0        0      150 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/error.py
+-rw-r--r--   0        0        0      460 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/logger.py
+-rw-r--r--   0        0        0     1101 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/main.py
+-rw-r--r--   0        0        0        0 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/__init__.py
+-rw-r--r--   0        0        0     1683 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/csv.py
+-rw-r--r--   0        0        0        0 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/mapper/__init__.py
+-rw-r--r--   0        0        0     1044 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/mapper/field.py
+-rw-r--r--   0        0        0      733 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/mapper/table.py
+-rw-r--r--   0        0        0        0 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/models/__init__.py
+-rw-r--r--   0        0        0      599 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/models/field.py
+-rw-r--r--   0        0        0      218 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/models/table.py
+-rw-r--r--   0        0        0     1161 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/reader/reader.py
+-rw-r--r--   0        0        0      755 2023-02-14 08:40:43.000000 odd_cli-0.1.9/odd_cli/tokens.py
+-rw-r--r--   0        0        0      813 2023-02-14 08:41:03.000000 odd_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 odd_cli-0.1.9/setup.py
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 odd_cli-0.1.9/PKG-INFO
```

### Comparing `odd_cli-0.1.8/LICENSE` & `odd_cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/README.md` & `odd_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/client.py` & `odd_cli-0.1.9/odd_cli/client.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/main.py` & `odd_cli-0.1.9/odd_cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 
 import typer
 from oddrn_generator.generators import FilesystemGenerator
 
 from odd_cli.client import Client
+from odd_cli.logger import logger
 from odd_cli.reader.reader import read
 from odd_cli.tokens import app as tokens_app
-from logger import logger
 
 app = typer.Typer()
 app.add_typer(
     tokens_app,
     name="tokens",
 )
```

### Comparing `odd_cli-0.1.8/odd_cli/reader/csv.py` & `odd_cli-0.1.9/odd_cli/reader/csv.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/reader/mapper/field.py` & `odd_cli-0.1.9/odd_cli/reader/mapper/field.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/reader/mapper/table.py` & `odd_cli-0.1.9/odd_cli/reader/mapper/table.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/reader/models/field.py` & `odd_cli-0.1.9/odd_cli/reader/models/field.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/reader/reader.py` & `odd_cli-0.1.9/odd_cli/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odd_cli-0.1.8/odd_cli/tokens.py` & `odd_cli-0.1.9/odd_cli/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 from requests import HTTPError
 from rich.console import Console
 
 from odd_cli.client import Client
-from logger import logger
+from odd_cli.logger import logger
 
 app = typer.Typer(short_help="Manipulate OpenDataDiscovery platform's tokens")
 err_console = Console(stderr=True)
 
 
 @app.command()
 def create(
```

### Comparing `odd_cli-0.1.8/pyproject.toml` & `odd_cli-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odd-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "Command line tool for working with OpenDataDiscovery. "
 authors = ["Pavel Makarichev <vixtir90@gmail.com>"]
 keywords=["Open Data Discovery", "Metadata", "Data Discovery", "Data Observability"]
 readme = "README.md"
 
 packages = [{include = "odd_cli"}]
```

### Comparing `odd_cli-0.1.8/setup.py` & `odd_cli-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['odd = odd_cli.main:app']}
 
 setup_kwargs = {
     'name': 'odd-cli',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Command line tool for working with OpenDataDiscovery. ',
     'long_description': "## OpenDataDiscovery CLI\n[![PyPI version](https://badge.fury.io/py/odd-cli.svg)](https://badge.fury.io/py/odd-cli)\n\nCommand line tool for working with OpenDataDiscovery. \nIt makes it easy to create token though console and ingest local dataset's metadata to OpenDataDiscovery platform.\n\n\n#### Available commands\n```text\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.                                              │\n│ --show-completion             Show completion for the current shell, to copy it or customize the installation        │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ─────────────────────────────────────────────────────────────────────────────────╮\n│ collect                       Collect and ingest metadata for local files from folder      │\n│ tokens                        Manipulate OpenDataDiscovery platform's tokens               │\n╰────────────────────────────────────────────────────────────────────────────────────────────╯\n```",
     'author': 'Pavel Makarichev',
     'author_email': 'vixtir90@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `odd_cli-0.1.8/PKG-INFO` & `odd_cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odd-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Command line tool for working with OpenDataDiscovery. 
 Keywords: Open Data Discovery,Metadata,Data Discovery,Data Observability
 Author: Pavel Makarichev
 Author-email: vixtir90@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

