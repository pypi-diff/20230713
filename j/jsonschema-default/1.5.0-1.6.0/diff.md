# Comparing `tmp/jsonschema-default-1.5.0.tar.gz` & `tmp/jsonschema_default-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema-default-1.5.0.tar", max compression
+gzip compressed data, was "jsonschema_default-1.6.0.tar", max compression
```

## Comparing `jsonschema-default-1.5.0.tar` & `jsonschema_default-1.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5356 2023-01-31 10:02:45.949602 jsonschema-default-1.5.0/jsonschema_default/__init__.py
--rw-r--r--   0        0        0    34523 2021-05-07 14:13:53.384529 jsonschema-default-1.5.0/LICENSE
--rw-r--r--   0        0        0      569 2023-01-31 10:03:41.570607 jsonschema-default-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      794 2021-05-07 14:13:53.384529 jsonschema-default-1.5.0/README.md
--rw-r--r--   0        0        0     1535 2023-01-31 10:05:55.447076 jsonschema-default-1.5.0/setup.py
--rw-r--r--   0        0        0     1572 2023-01-31 10:05:55.447076 jsonschema-default-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-07-10 08:17:48.950211 jsonschema_default-1.6.0/jsonschema_default/__init__.py
+-rw-r--r--   0        0        0     5408 2023-07-13 04:58:30.048621 jsonschema_default-1.6.0/jsonschema_default/main.py
+-rw-r--r--   0        0        0    34523 2021-05-07 14:13:53.384529 jsonschema_default-1.6.0/LICENSE
+-rw-r--r--   0        0        0      633 2023-07-13 04:59:45.821512 jsonschema_default-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      794 2021-05-07 14:13:53.384529 jsonschema_default-1.6.0/README.md
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 jsonschema_default-1.6.0/PKG-INFO
```

### Comparing `jsonschema-default-1.5.0/LICENSE` & `jsonschema_default-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema-default-1.5.0/pyproject.toml` & `jsonschema_default-1.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "jsonschema-default"
-version = "1.5.0"
+version = "1.6.0"
 description = "Create default objects from a JSON schema"
 authors = ["Martin Boos <mboos@outlook.com>"]
 maintainers = ["Martin Boos <mboos@outlook.com>"]
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/mnboos/jsonschema-default"
 license = "GNU AGPL v3"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-xeger = "^0.3.5"
+python = "^3.10"
+rstr = "^3.2.1"
+loguru = "^0.7.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.4.1"
-jsonschema = "^3.2.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+jsonschema = "^4.18.0"
+flake8 = "^6.0.0"
+black = "^23.7.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `jsonschema-default-1.5.0/README.md` & `jsonschema_default-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema-default-1.5.0/setup.py` & `jsonschema_default-1.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,56 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jsonschema-default
+Version: 1.6.0
+Summary: Create default objects from a JSON schema
+Home-page: https://github.com/mnboos/jsonschema-default
+License: GNU AGPL v3
+Author: Martin Boos
+Author-email: mboos@outlook.com
+Maintainer: Martin Boos
+Maintainer-email: mboos@outlook.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: rstr (>=3.2.1,<4.0.0)
+Project-URL: Repository, https://github.com/mnboos/jsonschema-default
+Description-Content-Type: text/markdown
+
+# jsonschema-instance
+
+A Python package that creates default objects from a JSON schema.
+
+## Note
+This is not a validator. Inputs should be valid JSON schemas. For Python you can use the [jsonschema](https://github.com/Julian/jsonschema) package to validate schemas.
+
+## Installation
+```
+pip install jsonschema-default
+```
+
+## Usage
+```python
+import jsonschema_default
+
+default_obj = jsonschema_default.create_from("<schema>")
+```
+
+## Development
+- Install and configure [Poetry](https://python-poetry.org/)
+
+```bash
+pip install --user poetry
+```
+
+See [Installation](https://python-poetry.org/docs/#installation) for the official guide.
+
+- Install the dependencies using 
+
+```bash
+# Configure poetry to create a local venv directory
+poetry config virtualenvs.in-project true
 
-packages = \
-['jsonschema_default']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['xeger>=0.3.5,<0.4.0']
-
-setup_kwargs = {
-    'name': 'jsonschema-default',
-    'version': '1.5.0',
-    'description': 'Create default objects from a JSON schema',
-    'long_description': '# jsonschema-instance\n\nA Python package that creates default objects from a JSON schema.\n\n## Note\nThis is not a validator. Inputs should be valid JSON schemas. For Python you can use the [jsonschema](https://github.com/Julian/jsonschema) package to validate schemas.\n\n## Installation\n```\npip install jsonschema-default\n```\n\n## Usage\n```python\nimport jsonschema_default\n\ndefault_obj = jsonschema_default.create_from("<schema>")\n```\n\n## Development\n- Install and configure [Poetry](https://python-poetry.org/)\n\n```bash\npip install --user poetry\n```\n\nSee [Installation](https://python-poetry.org/docs/#installation) for the official guide.\n\n- Install the dependencies using \n\n```bash\n# Configure poetry to create a local venv directory\npoetry config virtualenvs.in-project true\n\npoetry install\n```',
-    'author': 'Martin Boos',
-    'author_email': 'mboos@outlook.com',
-    'maintainer': 'Martin Boos',
-    'maintainer_email': 'mboos@outlook.com',
-    'url': 'https://github.com/mnboos/jsonschema-default',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+poetry install
+```
```

