# Comparing `tmp/mail-Generator-0.2.1.tar.gz` & `tmp/mail-Generator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail-Generator-0.2.1.tar", last modified: Thu Jul 13 14:33:26 2023, max compression
+gzip compressed data, was "mail-Generator-0.2.2.tar", last modified: Thu Jul 13 14:37:56 2023, max compression
```

## Comparing `mail-Generator-0.2.1.tar` & `mail-Generator-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:33:26.092437 mail-Generator-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 14:33:16.000000 mail-Generator-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:33:26.092437 mail-Generator-0.2.1/Mail_Generator/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 14:33:16.000000 mail-Generator-0.2.1/Mail_Generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-13 14:33:16.000000 mail-Generator-0.2.1/Mail_Generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 14:33:26.092437 mail-Generator-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-13 14:33:16.000000 mail-Generator-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:33:26.092437 mail-Generator-0.2.1/mail_Generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 14:33:26.000000 mail-Generator-0.2.1/mail_Generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:33:26.092437 mail-Generator-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-13 14:33:16.000000 mail-Generator-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:37:56.965433 mail-Generator-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 14:37:45.000000 mail-Generator-0.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:37:56.961433 mail-Generator-0.2.2/Mail_Generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 14:37:45.000000 mail-Generator-0.2.2/Mail_Generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-13 14:37:45.000000 mail-Generator-0.2.2/Mail_Generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-13 14:37:56.965433 mail-Generator-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-13 14:37:45.000000 mail-Generator-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:37:56.965433 mail-Generator-0.2.2/mail_Generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 14:37:56.000000 mail-Generator-0.2.2/mail_Generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:37:56.965433 mail-Generator-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 14:37:45.000000 mail-Generator-0.2.2/setup.py
```

### Comparing `mail-Generator-0.2.1/LICENSE` & `mail-Generator-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mail-Generator-0.2.1/Mail_Generator/main.py` & `mail-Generator-0.2.2/Mail_Generator/main.py`

 * *Files identical despite different names*

### Comparing `mail-Generator-0.2.1/PKG-INFO` & `mail-Generator-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Metadata-Version: 2.1
 Name: mail-Generator
-Version: 0.2.1
+Version: 0.2.2
+Summary: A Python package that provides an easy-to-use interface for creating and managing email addresses
+Home-page: https://github.com/matthieuEv/mail-generator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <a href="https://pypi.org/project/mail-Generator/" target="_blank">
     <img src="https://github.com/matthieuEv/mail-generator/blob/main/logo.png?raw=true" alt="Logo" width="300">
   </a>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-Metadata-Version: 2.1 Name: mail-Generator Version: 0.2.1 Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: mail-Generator Version: 0.2.2 Summary: A Python
+package that provides an easy-to-use interface for creating and managing email
+addresses Home-page: https://github.com/matthieuEv/mail-generator Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
 # Mail-generator ![GitHub Workflow Status (with event)](https://img.shields.io/
 github/actions/workflow/status/matthieuEv/mail-generator/python-
 publish.yml?style=for-the-badge&color=%230a41a8) ![Static Badge](https://
 img.shields.io/badge/Mail--Generator%20on%20PyPI-230a41a8?style=for-the-
 badge&color=%230a41a8&link=https%3A%2F%2Fpypi.org%2Fproject%2Fmail-
 Generator%2F) ## Description `Mail-Generator` is a Python package that provides
```

### Comparing `mail-Generator-0.2.1/README.md` & `mail-Generator-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mail-Generator-0.2.1/mail_Generator.egg-info/PKG-INFO` & `mail-Generator-0.2.2/mail_Generator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Metadata-Version: 2.1
 Name: mail-Generator
-Version: 0.2.1
+Version: 0.2.2
+Summary: A Python package that provides an easy-to-use interface for creating and managing email addresses
+Home-page: https://github.com/matthieuEv/mail-generator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <a href="https://pypi.org/project/mail-Generator/" target="_blank">
     <img src="https://github.com/matthieuEv/mail-generator/blob/main/logo.png?raw=true" alt="Logo" width="300">
   </a>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-Metadata-Version: 2.1 Name: mail-Generator Version: 0.2.1 Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: mail-Generator Version: 0.2.2 Summary: A Python
+package that provides an easy-to-use interface for creating and managing email
+addresses Home-page: https://github.com/matthieuEv/mail-generator Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
 # Mail-generator ![GitHub Workflow Status (with event)](https://img.shields.io/
 github/actions/workflow/status/matthieuEv/mail-generator/python-
 publish.yml?style=for-the-badge&color=%230a41a8) ![Static Badge](https://
 img.shields.io/badge/Mail--Generator%20on%20PyPI-230a41a8?style=for-the-
 badge&color=%230a41a8&link=https%3A%2F%2Fpypi.org%2Fproject%2Fmail-
 Generator%2F) ## Description `Mail-Generator` is a Python package that provides
```

