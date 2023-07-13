# Comparing `tmp/openhexa.toolbox-0.1.1.tar.gz` & `tmp/openhexa.toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.1.1.tar", last modified: Thu Jul 13 11:13:15 2023, max compression
+gzip compressed data, was "openhexa.toolbox-0.1.2.tar", last modified: Thu Jul 13 11:43:25 2023, max compression
```

## Comparing `openhexa.toolbox-0.1.1.tar` & `openhexa.toolbox-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:13:15.788383 openhexa.toolbox-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 11:12:47.000000 openhexa.toolbox-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:13:15.788383 openhexa.toolbox-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:12:47.000000 openhexa.toolbox-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:13:15.788383 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:13:15.000000 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-13 11:13:15.000000 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:13:15.000000 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 11:13:15.000000 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 11:13:15.000000 openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-13 11:12:47.000000 openhexa.toolbox-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:13:15.788383 openhexa.toolbox-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29915 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/setup.cfg
```

### Comparing `openhexa.toolbox-0.1.1/LICENSE` & `openhexa.toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.1/PKG-INFO` & `openhexa.toolbox-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.1/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.1/pyproject.toml` & `openhexa.toolbox-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.1.1"
+version = "0.1.2"
 description = "A set of tools to acquire & process data from various sources"
 authors = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com"}
 ]
 maintainers = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com" }
 ]
@@ -29,20 +29,16 @@
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "build"]
 
 [tool.setuptools.packages.find]
 where = ["."]
-include = ["openhexa"]
 namespaces = true
 
-[tool.setuptools]
-py-modules = []
-
 [project.urls]
 "Homepage" = "https://github.com/blsq/openhexa-toolbox"
 "Bug Tracker" = "https://github.com/blsq/openhexa-toolbox/issues"
 
 [tool.black]
 line-length = 88
```

