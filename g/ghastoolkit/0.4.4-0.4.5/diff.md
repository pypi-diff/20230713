# Comparing `tmp/ghastoolkit-0.4.4.tar.gz` & `tmp/ghastoolkit-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.4.tar", last modified: Wed Jul  5 10:53:35 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.5.tar", last modified: Thu Jul 13 17:06:51 2023, max compression
```

## Comparing `ghastoolkit-0.4.4.tar` & `ghastoolkit-0.4.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.125151 ghastoolkit-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.125151 ghastoolkit-0.4.5/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.133151 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.129151 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 17:06:51.000000 ghastoolkit-0.4.5/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:51.137151 ghastoolkit-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 17:06:13.000000 ghastoolkit-0.4.5/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.4/LICENSE` & `ghastoolkit-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/PKG-INFO` & `ghastoolkit-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.4
+Version: 0.4.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.4/README.md` & `ghastoolkit-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/pyproject.toml` & `ghastoolkit-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "certifi==2023.5.7",
-    "charset-normalizer==3.1.0",
+    "charset-normalizer==3.2.0",
     "idna==3.4",
     "PyYAML==6.0",
     "ratelimit==2.2.1",
     "requests==2.31.0",
     "urllib3==2.0.3"
 ]
```

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.5/src/ghastoolkit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.5/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.5/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/codescanning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 import json
 import logging
-from typing import Any, Optional
+from typing import Any, List, Optional
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import OctoItem, RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
 @dataclass
@@ -17,33 +17,33 @@
 
     rule: dict
     tool: dict
 
     _instances: Optional[list[dict]] = None
 
     @property
-    def rule_id(self):
-        return self.rule.get("id")
+    def rule_id(self) -> str:
+        return self.rule.get("id", "NA")
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         return self.rule.get("description")
 
     @property
-    def tool_name(self):
-        return self.tool.get("name")
+    def tool_name(self) -> str:
+        return self.tool.get("name", "NA")
 
     @property
-    def tool_fullname(self):
+    def tool_fullname(self) -> str:
         version = self.tool.get("version")
         return f"{self.tool_name}@{version}"
 
     @property
-    def severity(self):
-        return self.rule.get("severity")
+    def severity(self) -> str:
+        return self.rule.get("severity", "NA")
 
     @property
     def instances(self) -> list[dict]:
         if not self._instances:
             self._instances = CodeScanning().getAlertInstances(self.number)
         return self._instances
 
@@ -54,14 +54,16 @@
 class CodeScanning:
     def __init__(self, repository: Optional[Repository] = None) -> None:
         """GitHub Code Scanning REST API
 
         https://docs.github.com/en/rest/code-scanning
         """
         self.repository = repository or GitHub.repository
+        self.tools: List[str] = []
+
         if not self.repository:
             raise Exception("CodeScanning requires Repository to be set")
         self.rest = RestRequest(self.repository)
 
     def getOrganizationAlerts(self, state: str = "open") -> list[dict[Any, Any]]:
         """Get Organization Alerts
 
@@ -84,15 +86,15 @@
         ref: Optional[str] = None,
     ) -> list[CodeAlert]:
         """Get all code scanning alerts
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-a-repository
         """
         return []
 
-    def getAlertsInPR(self, base: str) -> list[dict]:
+    def getAlertsInPR(self, base: str) -> list[CodeAlert]:
         """Get the open alerts in a Pull Request (delta / diff).
 
         Note this operation is slow due to it needing to lookup each alert instance
         information.
 
         base: str - Base reference
         https://docs.github.com/en/rest/code-scanning#list-instances-of-a-code-scanning-alert
@@ -109,15 +111,15 @@
             if len(alert_info) == 0:
                 results.append(alert)
         return results
 
     @RestRequest.restGet(
         "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}", authenticated=True
     )
-    def getAlert(self, alert_number: int) -> dict:
+    def getAlert(self, alert_number: int) -> CodeAlert:
         """Get Single Alert
         https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
         """
         return {}
 
     def getAlertInstances(
         self, alert_number: int, ref: Optional[str] = None
@@ -151,16 +153,24 @@
         for analysis in self.getAnalyses(reference, tool):
             name = analysis.get("tool", {}).get("name")
             if name in tools:
                 continue
             tools.add(name)
             results.append(analysis)
 
+        self.tools = list(tools)
+
         return results
 
+    def getTools(self, reference: Optional[str] = None) -> List[str]:
+        """Get list of tools from the latest analyses"""
+        if len(self.tools) == 0:
+            self.getLatestAnalyses(reference)
+        return self.tools
+
     def getSarifId(self, url: str) -> int:
         """Get the latest SARIF ID from a URL"""
         if url and "/" in url:
             return int(url.split("/")[-1])
         return -1
 
     def downloadSARIF(self, output: str, sarif_id: int) -> bool:
```

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.5/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.5/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.5/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.5/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.4
+Version: 0.4.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.4/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.5/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_codeql_dataext.py` & `ghastoolkit-0.4.5/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_codeqldb.py` & `ghastoolkit-0.4.5/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_codescanning.py` & `ghastoolkit-0.4.5/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_default.py` & `ghastoolkit-0.4.5/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_dependencies.py` & `ghastoolkit-0.4.5/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_depgraph.py` & `ghastoolkit-0.4.5/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_github.py` & `ghastoolkit-0.4.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_licenses.py` & `ghastoolkit-0.4.5/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_octokit.py` & `ghastoolkit-0.4.5/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.4/tests/test_secretscanning.py` & `ghastoolkit-0.4.5/tests/test_secretscanning.py`

 * *Files identical despite different names*

