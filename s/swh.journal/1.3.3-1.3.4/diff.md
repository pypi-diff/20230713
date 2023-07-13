# Comparing `tmp/swh.journal-1.3.3.tar.gz` & `tmp/swh.journal-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.journal-1.3.3.tar", last modified: Fri May  5 11:43:48 2023, max compression
+gzip compressed data, was "swh.journal-1.3.4.tar", last modified: Thu Jul 13 08:03:33 2023, max compression
```

## Comparing `swh.journal-1.3.3.tar` & `swh.journal-1.3.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-05 11:43:46.000000 swh.journal-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-05 11:43:46.000000 swh.journal-1.3.3/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-05 11:43:46.000000 swh.journal-1.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-05 11:43:46.000000 swh.journal-1.3.3/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-05 11:43:46.000000 swh.journal-1.3.3/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-05-05 11:43:46.000000 swh.journal-1.3.3/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-05 11:43:46.000000 swh.journal-1.3.3/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-05 11:43:48.000000 swh.journal-1.3.3/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-05-05 11:43:46.000000 swh.journal-1.3.3/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-05-05 11:43:46.000000 swh.journal-1.3.3/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-05-05 11:43:46.000000 swh.journal-1.3.3/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-05 11:43:46.000000 swh.journal-1.3.3/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-05-05 11:43:46.000000 swh.journal-1.3.3/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      382 2023-05-05 11:43:46.000000 swh.journal-1.3.3/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-05 11:43:48.000000 swh.journal-1.3.3/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-05-05 11:43:46.000000 swh.journal-1.3.3/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17402 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     7859 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) docker     (999)    18361 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-05 11:43:46.000000 swh.journal-1.3.3/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-05 11:43:48.000000 swh.journal-1.3.3/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-05-05 11:43:46.000000 swh.journal-1.3.3/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-13 08:03:27.000000 swh.journal-1.3.4/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-13 08:03:27.000000 swh.journal-1.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-13 08:03:27.000000 swh.journal-1.3.4/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-13 08:03:27.000000 swh.journal-1.3.4/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-07-13 08:03:27.000000 swh.journal-1.3.4/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-13 08:03:27.000000 swh.journal-1.3.4/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-13 08:03:33.392235 swh.journal-1.3.4/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-07-13 08:03:27.000000 swh.journal-1.3.4/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-07-13 08:03:27.000000 swh.journal-1.3.4/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-13 08:03:27.000000 swh.journal-1.3.4/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-07-13 08:03:27.000000 swh.journal-1.3.4/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      405 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-13 08:03:33.392235 swh.journal-1.3.4/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-07-13 08:03:27.000000 swh.journal-1.3.4/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh/journal/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18355 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     7860 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) docker     (999)    19253 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      146 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-07-13 08:03:27.000000 swh.journal-1.3.4/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.journal-1.3.3/.pre-commit-config.yaml` & `swh.journal-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/CODE_OF_CONDUCT.md` & `swh.journal-1.3.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/LICENSE` & `swh.journal-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/PKG-INFO` & `swh.journal-1.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.3
+Version: 1.3.4
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.3/README.md` & `swh.journal-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/docs/example-journal-client.py` & `swh.journal-1.3.4/docs/example-journal-client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/docs/journal-clients.rst` & `swh.journal-1.3.4/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/setup.py` & `swh.journal-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/client.py` & `swh.journal-1.3.4/swh/journal/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from confluent_kafka import (
     OFFSET_BEGINNING,
     Consumer,
     KafkaError,
     KafkaException,
     TopicPartition,
 )
+from confluent_kafka.admin import AdminClient, NewTopic
 
 from swh.core.statsd import Statsd
 from swh.journal import DEFAULT_PREFIX
 
 from .serializers import kafka_to_value
 
 logger = logging.getLogger(__name__)
@@ -132,14 +133,16 @@
             stop, or restart from earliest offsets); defaults to continuing.
             This can be either a :class:`EofBehavior` variant or a string containing the
             name of one of the variants.
         stop_on_eof: (deprecated) equivalent to passing ``on_eof=EofBehavior.STOP``
         auto_offset_reset: sets the behavior of the client when the consumer group
             initializes: ``'earliest'`` (the default) processes all objects since the
             inception of the topics; ``''``
+        create_topics: Create kafka topics if they do not exist, not for production, this
+            flag should only be enabled in development environments.
 
     Any other named argument is passed directly to KafkaConsumer().
 
     """
 
     def __init__(
         self,
@@ -151,14 +154,15 @@
         stop_after_objects: Optional[int] = None,
         batch_size: int = 200,
         process_timeout: Optional[float] = None,
         auto_offset_reset: str = "earliest",
         stop_on_eof: Optional[bool] = None,
         on_eof: Optional[Union[EofBehavior, str]] = None,
         value_deserializer: Optional[Callable[[str, bytes], Any]] = None,
+        create_topics: bool = False,
         **kwargs,
     ):
         if prefix is None:
             prefix = DEFAULT_PREFIX
         if auto_offset_reset not in ACCEPTED_OFFSET_RESET:
             raise ValueError(
                 "Option 'auto_offset_reset' only accept %s, not %s"
@@ -265,33 +269,51 @@
             topic
             for topic in self.consumer.list_topics(timeout=10).topics.keys()
             if (
                 topic.startswith(f"{prefix}.")
                 or topic.startswith(f"{privileged_prefix}.")
             )
         ]
-        if not existing_topics:
+
+        if not create_topics and not existing_topics:
             raise ValueError(
                 f"The prefix {prefix} does not match any existing topic "
                 "on the kafka broker"
             )
 
         if not object_types:
             object_types = list({topic.split(".")[-1] for topic in existing_topics})
 
         self.subscription = []
         unknown_types = []
         for object_type in object_types:
             topics = (f"{privileged_prefix}.{object_type}", f"{prefix}.{object_type}")
             for topic in topics:
-                if topic in existing_topics:
+                if create_topics or topic in existing_topics:
                     self.subscription.append(topic)
                     break
             else:
                 unknown_types.append(object_type)
+
+        if create_topics:
+            topic_list = [
+                NewTopic(topic, 1, 1)
+                for topic in self.subscription
+                if topic not in existing_topics
+            ]
+            logger.debug("Creating topics: %s", topic_list)
+            admin_client = AdminClient({"bootstrap.servers": ",".join(brokers)})
+            for topic in admin_client.create_topics(topic_list).values():
+                try:
+                    # wait for topic to be created
+                    topic.result()  # type: ignore[attr-defined]
+                except KafkaException:
+                    # topic already exists
+                    pass
+
         if unknown_types:
             raise ValueError(
                 f"Topic(s) for object types {','.join(unknown_types)} "
                 "are unknown on the kafka broker"
             )
 
         logger.debug(f"Upstream topics: {existing_topics}")
```

### Comparing `swh.journal-1.3.3/swh/journal/pytest_plugin.py` & `swh.journal-1.3.4/swh/journal/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     object_type from the ``privileged_object_types`` list.
 
     """
     topics = [f"{kafka_prefix}.{obj}" for obj in object_types] + [
         f"{kafka_prefix}_privileged.{obj}" for obj in privileged_object_types
     ]
 
-    # unfortunately, the Mock broker does not support the CreatTopic admin API, so we
+    # unfortunately, the Mock broker does not support the CreateTopic admin API, so we
     # have to create topics using a Producer.
     producer = Producer(
         {
             "bootstrap.servers": kafka_server_base,
             "client.id": "bootstrap producer",
             "acks": "all",
         }
```

### Comparing `swh.journal-1.3.3/swh/journal/serializers.py` & `swh.journal-1.3.4/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/journal_data.py` & `swh.journal-1.3.4/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_client.py` & `swh.journal-1.3.4/swh/journal/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -350,15 +350,15 @@
 
     producer.flush()
 
     client = JournalClient(
         brokers=[kafka_server],
         group_id=kafka_consumer_group,
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         batch_size=batch_size,
     )
 
     collected_output: List[Dict] = []
 
     def worker_fn(objects):
         received = objects["content"]
@@ -402,15 +402,15 @@
 def test_client_subscribe_all(
     kafka_producer: Producer, kafka_prefix: str, kafka_server_base: str
 ):
     client = JournalClient(
         brokers=[kafka_server_base],
         group_id="whatever",
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
     )
     assert set(client.subscription) == {
         f"{kafka_prefix}.something",
         f"{kafka_prefix}.else",
     }
 
     worker_fn = MagicMock()
@@ -426,15 +426,15 @@
 def test_client_subscribe_one_topic(
     kafka_producer: Producer, kafka_prefix: str, kafka_server_base: str
 ):
     client = JournalClient(
         brokers=[kafka_server_base],
         group_id="whatever",
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         object_types=["else"],
     )
     assert client.subscription == [f"{kafka_prefix}.else"]
 
     worker_fn = MagicMock()
     client.process(worker_fn)
     worker_fn.assert_called_once_with({"else": ["value2"]})
@@ -444,35 +444,35 @@
     kafka_producer: Producer, kafka_prefix: str, kafka_server_base: str
 ):
     with pytest.raises(ValueError):
         JournalClient(
             brokers=[kafka_server_base],
             group_id="whatever",
             prefix=kafka_prefix,
-            stop_on_eof=True,
+            on_eof=EofBehavior.STOP,
             object_types=["really"],
         )
 
 
 def test_client_subscribe_absent_prefix(
     kafka_producer: Producer, kafka_prefix: str, kafka_server_base: str
 ):
     with pytest.raises(ValueError):
         JournalClient(
             brokers=[kafka_server_base],
             group_id="whatever",
             prefix="wrong.prefix",
-            stop_on_eof=True,
+            on_eof=EofBehavior.STOP,
         )
     with pytest.raises(ValueError):
         JournalClient(
             brokers=[kafka_server_base],
             group_id="whatever",
             prefix="wrong.prefix",
-            stop_on_eof=True,
+            on_eof=EofBehavior.STOP,
             object_types=["else"],
         )
 
 
 def test_client_subscriptions_with_anonymized_topics(
     kafka_prefix: str, kafka_consumer_group: str, kafka_server_base: str
 ):
@@ -499,15 +499,15 @@
     producer.flush()
 
     # without privileged "channels" activated on the client side
     client = JournalClient(
         brokers=[kafka_server_base],
         group_id=kafka_consumer_group,
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         privileged=False,
     )
     # we only subscribed to "standard" topics
     assert client.subscription == [kafka_prefix + ".revision"]
 
     # with privileged "channels" activated on the client side
     client = JournalClient(
@@ -540,26 +540,26 @@
     producer.flush()
 
     # without privileged channel activated on the client side
     client = JournalClient(
         brokers=[kafka_server_base],
         group_id=kafka_consumer_group,
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         privileged=False,
     )
     # we only subscribed to the standard prefix
     assert client.subscription == [kafka_prefix + ".revision"]
 
     # with privileged channel activated on the client side
     client = JournalClient(
         brokers=[kafka_server_base],
         group_id=kafka_consumer_group,
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         privileged=True,
     )
     # we also only subscribed to the standard prefix, since there is no priviled prefix
     # on the kafka broker
     assert client.subscription == [kafka_prefix + ".revision"]
 
 
@@ -592,21 +592,47 @@
             return None
         return Revision.from_dict(obj)
 
     client = JournalClient(
         brokers=[kafka_server],
         group_id=kafka_consumer_group,
         prefix=kafka_prefix,
-        stop_on_eof=True,
+        on_eof=EofBehavior.STOP,
         value_deserializer=custom_deserializer,
     )
     worker_fn = MagicMock()
     client.process(worker_fn)
 
     # a commit seems to be needed to prevent some race condition situation
     # where the worker_fn has not yet been called at this point (not sure how)
     client.consumer.commit()
 
     # Check the first revision has not been passed to worker_fn
     processed_revisions = set(worker_fn.call_args[0][0]["revision"])
     assert revisions[0] not in processed_revisions
     assert all(rev in processed_revisions for rev in revisions[1:])
+
+
+def test_client_create_topics(
+    kafka_prefix: str, kafka_consumer_group: str, kafka_server_base: str, mocker
+):
+
+    # the Mock broker does not support the CreateTopic admin API, so we
+    # mock the call to AdminClient.create_topics
+    mock_admin = mocker.patch("swh.journal.client.AdminClient")
+    mock_topic_future = mocker.Mock()
+    mock_topic_future.result.return_value = None
+    mock_admin.create_topics.return_value = {
+        kafka_prefix + ".revision": mock_topic_future
+    }
+
+    client = JournalClient(
+        brokers=[kafka_server_base],
+        group_id=kafka_consumer_group,
+        prefix=kafka_prefix,
+        on_eof=EofBehavior.STOP,
+        privileged=False,
+        object_types=["revision"],
+        create_topics=True,
+    )
+
+    assert client.subscription == [kafka_prefix + ".revision"]
```

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_inmemory.py` & `swh.journal-1.3.4/swh/journal/tests/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_kafka_writer.py` & `swh.journal-1.3.4/swh/journal/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_pytest_plugin.py` & `swh.journal-1.3.4/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_serializers.py` & `swh.journal-1.3.4/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/tests/test_stream.py` & `swh.journal-1.3.4/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/writer/__init__.py` & `swh.journal-1.3.4/swh/journal/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/writer/inmemory.py` & `swh.journal-1.3.4/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/writer/interface.py` & `swh.journal-1.3.4/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/writer/kafka.py` & `swh.journal-1.3.4/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh/journal/writer/stream.py` & `swh.journal-1.3.4/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/swh.journal.egg-info/PKG-INFO` & `swh.journal-1.3.4/swh.journal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.3
+Version: 1.3.4
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.3/swh.journal.egg-info/SOURCES.txt` & `swh.journal-1.3.4/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.3/tox.ini` & `swh.journal-1.3.4/tox.ini`

 * *Files identical despite different names*

