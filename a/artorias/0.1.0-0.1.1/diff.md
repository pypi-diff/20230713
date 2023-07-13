# Comparing `tmp/artorias-0.1.0.tar.gz` & `tmp/artorias-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artorias-0.1.0.tar", max compression
+gzip compressed data, was "artorias-0.1.1.tar", max compression
```

## Comparing `artorias-0.1.0.tar` & `artorias-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.0/artorias/__init__.py
--rw-r--r--   0        0        0      822 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.0/artorias/web/__init__.py
--rw-r--r--   0        0        0       23 2023-06-21 05:31:04.248093 artorias-0.1.0/artorias/web/flask/__init__.py
--rw-r--r--   0        0        0     2906 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/app.py
--rw-r--r--   0        0        0      496 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/celery.py
--rw-r--r--   0        0        0      208 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/exts.py
--rw-r--r--   0        0        0      120 2023-06-21 05:30:20.191515 artorias-0.1.0/artorias/web/flask/json.py
--rw-r--r--   0        0        0      429 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/settings.py
--rw-r--r--   0        0        0      657 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/sqlalchemy.py
--rw-r--r--   0        0        0      416 2023-07-13 07:40:04.671720 artorias-0.1.0/artorias/web/flask/utils.py
--rw-r--r--   0        0        0      586 2023-07-13 07:40:04.675720 artorias-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 artorias-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 08:31:07.627451 artorias-0.1.1/artorias/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.1/artorias/web/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-21 05:31:04.248093 artorias-0.1.1/artorias/web/flask/__init__.py
+-rw-r--r--   0        0        0     2906 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/app.py
+-rw-r--r--   0        0        0      496 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/celery.py
+-rw-r--r--   0        0        0      208 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/exts.py
+-rw-r--r--   0        0        0      120 2023-06-21 05:30:20.191515 artorias-0.1.1/artorias/web/flask/json.py
+-rw-r--r--   0        0        0      429 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/settings.py
+-rw-r--r--   0        0        0      657 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/sqlalchemy.py
+-rw-r--r--   0        0        0      416 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/utils.py
+-rw-r--r--   0        0        0      611 2023-07-13 08:30:42.235315 artorias-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 artorias-0.1.1/PKG-INFO
```

### Comparing `artorias-0.1.0/artorias/utils/__init__.py` & `artorias-0.1.1/artorias/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `artorias-0.1.0/artorias/web/flask/app.py` & `artorias-0.1.1/artorias/web/flask/app.py`

 * *Files identical despite different names*

### Comparing `artorias-0.1.0/artorias/web/flask/sqlalchemy.py` & `artorias-0.1.1/artorias/web/flask/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `artorias-0.1.0/pyproject.toml` & `artorias-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "artorias"
-version = "0.1.0"
+version = "0.1.1"
 description = "My web utilities"
 authors = ["Abyssknight <501835725@qq.com>"]
 readme = "README.md"
+include = ["artorias/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 flask = "^2.3.2"
 sqlalchemy = "^2.0.12"
 flask-shell-ipython = "^0.5.1"
 flask-sqlalchemy = "^3.0.3"
```

### Comparing `artorias-0.1.0/PKG-INFO` & `artorias-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artorias
-Version: 0.1.0
+Version: 0.1.1
 Summary: My web utilities
 Author: Abyssknight
 Author-email: 501835725@qq.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
```

