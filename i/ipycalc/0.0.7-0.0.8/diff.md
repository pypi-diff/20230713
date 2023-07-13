# Comparing `tmp/ipycalc-0.0.7.tar.gz` & `tmp/ipycalc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipycalc-0.0.7.tar", last modified: Fri Sep 23 16:32:21 2022, max compression
+gzip compressed data, was "ipycalc-0.0.8.tar", last modified: Thu Sep 29 02:01:07 2022, max compression
```

## Comparing `ipycalc-0.0.7.tar` & `ipycalc-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:32:21.296232 ipycalc-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-23 16:32:14.000000 ipycalc-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-23 16:32:21.296232 ipycalc-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:32:14.000000 ipycalc-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:32:21.296232 ipycalc-0.0.7/ipycalc/
--rw-r--r--   0 runner    (1001) docker     (121)    21787 2022-09-23 16:32:14.000000 ipycalc-0.0.7/ipycalc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:32:21.296232 ipycalc-0.0.7/ipycalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-23 16:32:21.000000 ipycalc-0.0.7/ipycalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-23 16:32:21.000000 ipycalc-0.0.7/ipycalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 16:32:21.000000 ipycalc-0.0.7/ipycalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-23 16:32:21.000000 ipycalc-0.0.7/ipycalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-23 16:32:21.000000 ipycalc-0.0.7/ipycalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 16:32:21.296232 ipycalc-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-09-23 16:32:14.000000 ipycalc-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 02:01:07.865113 ipycalc-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-29 02:01:00.000000 ipycalc-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-29 02:01:07.865113 ipycalc-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 02:01:00.000000 ipycalc-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 02:01:07.865113 ipycalc-0.0.8/ipycalc/
+-rw-r--r--   0 runner    (1001) docker     (121)    21772 2022-09-29 02:01:00.000000 ipycalc-0.0.8/ipycalc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 02:01:07.865113 ipycalc-0.0.8/ipycalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-29 02:01:07.000000 ipycalc-0.0.8/ipycalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-29 02:01:07.000000 ipycalc-0.0.8/ipycalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 02:01:07.000000 ipycalc-0.0.8/ipycalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-29 02:01:07.000000 ipycalc-0.0.8/ipycalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-29 02:01:07.000000 ipycalc-0.0.8/ipycalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-29 02:01:07.865113 ipycalc-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-09-29 02:01:00.000000 ipycalc-0.0.8/setup.py
```

### Comparing `ipycalc-0.0.7/LICENSE` & `ipycalc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipycalc-0.0.7/ipycalc/__init__.py` & `ipycalc-0.0.8/ipycalc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,23 +411,23 @@
     
     # Split the 'if' portion into the condition and value
     value, condition = if_text.split('if', 1)
 
     # Check if the 'if' is an really an 'if' or if it's an 'elif'
     if type == 'if':
         # Add an 'if' line
-        latex_text = value + '\\textsf{@if@}' + condition + '\\newline'
+        latex_text = value + '\\textsf{@if@}' + condition + '\\\\'
     elif type == 'elif':
         # Add an 'else if' line
-        latex_text = '\\hspace{1cm}'  + '\\textsf{else@}' + value + '\\textsf{@if@}' + condition + '\\newline'
+        latex_text = '\\hspace{1cm}'  + '\\textsf{else@}' + value + '\\textsf{@if@}' + condition + '\\\\'
 
     # Check for an 'else' condition without an 'if' in it
     if '@if@' not in else_text:
         # Add the 'else' text
-        latex_text += '\\hspace{1cm}' + '\\textsf{else@}' + else_text + '\\newline'
+        latex_text += '\\hspace{1cm}' + '\\textsf{else@}' + else_text + '\\\\'
     
     # Evaluate 'if' statements nested in the 'else' statement
     elif else_text != '':
 
         # Remove any whitespace at the ends of the else text
         else_text = else_text.strip()
```

### Comparing `ipycalc-0.0.7/setup.py` & `ipycalc-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipycalc",
-    version="0.0.7",
+    version="0.0.8",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="Clean looking engineering calculations for IPython",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/ipycalc.git",
     packages=setuptools.find_packages(include=['ipycalc', 'ipycalc.*']),
```

