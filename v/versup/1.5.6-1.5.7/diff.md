# Comparing `tmp/versup-1.5.6.tar.gz` & `tmp/versup-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versup-1.5.6.tar", max compression
+gzip compressed data, was "versup-1.5.7.tar", max compression
```

## Comparing `versup-1.5.6.tar` & `versup-1.5.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1071 2022-10-27 09:52:52.245581 versup-1.5.6/LICENSE.txt
--rw-r--r--   0        0        0     6276 2022-10-27 09:52:52.245581 versup-1.5.6/README.md
--rw-r--r--   0        0        0      745 2023-01-05 10:35:47.550396 versup-1.5.6/pyproject.toml
--rw-r--r--   0        0        0      225 2023-01-05 10:35:47.550396 versup-1.5.6/versup/__init__.py
--rw-r--r--   0        0        0      112 2022-10-27 09:52:52.245581 versup-1.5.6/versup/__main__.py
--rw-r--r--   0        0        0     2815 2022-12-16 16:08:19.093777 versup-1.5.6/versup/changelog.py
--rw-r--r--   0        0        0     8139 2022-12-16 16:01:11.623775 versup-1.5.6/versup/command_line.py
--rw-r--r--   0        0        0     1813 2022-12-16 16:01:11.623775 versup-1.5.6/versup/conf_reader.py
--rw-r--r--   0        0        0     1058 2022-10-27 09:52:52.245581 versup-1.5.6/versup/custom_cmd_group.py
--rw-r--r--   0        0        0     2403 2022-10-27 09:52:52.245581 versup-1.5.6/versup/default_conf.py
--rw-r--r--   0        0        0     2908 2022-12-16 16:09:38.063778 versup-1.5.6/versup/file_updater.py
--rw-r--r--   0        0        0     4045 2023-01-05 10:31:04.040393 versup-1.5.6/versup/gitops.py
--rw-r--r--   0        0        0      328 2022-10-27 09:52:52.245581 versup-1.5.6/versup/printer.py
--rw-r--r--   0        0        0     1531 2022-12-16 16:10:35.783778 versup-1.5.6/versup/script_runner.py
--rw-r--r--   0        0        0      677 2022-12-16 16:10:06.653779 versup-1.5.6/versup/template.py
--rw-r--r--   0        0        0     1656 2022-12-16 16:01:11.623775 versup-1.5.6/versup/versioning.py
--rw-r--r--   0        0        0     7298 1970-01-01 00:00:00.000000 versup-1.5.6/setup.py
--rw-r--r--   0        0        0     7109 1970-01-01 00:00:00.000000 versup-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 17:32:13.791297 versup-1.5.7/LICENSE.txt
+-rw-r--r--   0        0        0     6276 2023-07-13 17:32:13.795297 versup-1.5.7/README.md
+-rw-r--r--   0        0        0      745 2023-07-13 17:35:54.704031 versup-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-07-13 17:35:54.704031 versup-1.5.7/versup/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-13 17:32:13.799297 versup-1.5.7/versup/__main__.py
+-rw-r--r--   0        0        0     2815 2023-07-13 17:32:13.799297 versup-1.5.7/versup/changelog.py
+-rw-r--r--   0        0        0     8139 2023-07-13 17:32:13.799297 versup-1.5.7/versup/command_line.py
+-rw-r--r--   0        0        0     1813 2023-07-13 17:32:13.799297 versup-1.5.7/versup/conf_reader.py
+-rw-r--r--   0        0        0     1058 2023-07-13 17:32:13.799297 versup-1.5.7/versup/custom_cmd_group.py
+-rw-r--r--   0        0        0     2401 2023-07-13 17:32:13.799297 versup-1.5.7/versup/default_conf.py
+-rw-r--r--   0        0        0     2908 2023-07-13 17:32:13.799297 versup-1.5.7/versup/file_updater.py
+-rw-r--r--   0        0        0     4045 2023-07-13 17:32:13.799297 versup-1.5.7/versup/gitops.py
+-rw-r--r--   0        0        0      328 2023-07-13 17:32:13.799297 versup-1.5.7/versup/printer.py
+-rw-r--r--   0        0        0     1531 2023-07-13 17:32:13.799297 versup-1.5.7/versup/script_runner.py
+-rw-r--r--   0        0        0      677 2023-07-13 17:32:13.799297 versup-1.5.7/versup/template.py
+-rw-r--r--   0        0        0     1656 2023-07-13 17:32:13.799297 versup-1.5.7/versup/versioning.py
+-rw-r--r--   0        0        0     7109 1970-01-01 00:00:00.000000 versup-1.5.7/PKG-INFO
```

### Comparing `versup-1.5.6/LICENSE.txt` & `versup-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/README.md` & `versup-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/pyproject.toml` & `versup-1.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "versup"
-version = "1.5.6"
+version = "1.5.7"
 description = "Version up your project with ease."
 authors = ["Sven Steinbauer <sven@unlogic.co.uk>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Svenito/versup"
 
 [tool.poetry.dependencies]
```

### Comparing `versup-1.5.6/versup/changelog.py` & `versup-1.5.7/versup/changelog.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/command_line.py` & `versup-1.5.7/versup/command_line.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/conf_reader.py` & `versup-1.5.7/versup/conf_reader.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/custom_cmd_group.py` & `versup-1.5.7/versup/custom_cmd_group.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/default_conf.py` & `versup-1.5.7/versup/default_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         "version": "### Version [version]",  # Template for the version line
         "commit": "- [message]",  # Template for the commit line
         "separator": "\n",  # Template for the separator between versions sections
     },
     "commit": {
         "enabled": True,  # Commit the changes automatically
         "message": "Update version to [version]",  # Template for the commit message
-        "mainbranch": "master",  # name of the main development or release branch
+        "mainbranch": "main",  # name of the main development or release branch
     },
     "tag": {
         "enabled": True,  # Tag the bump commit
         "name": "v[version]",  # Template for the name of the tag in the tag message
     },
     "tokens": {
         "date": {
```

### Comparing `versup-1.5.6/versup/file_updater.py` & `versup-1.5.7/versup/file_updater.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/gitops.py` & `versup-1.5.7/versup/gitops.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/script_runner.py` & `versup-1.5.7/versup/script_runner.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/template.py` & `versup-1.5.7/versup/template.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/versup/versioning.py` & `versup-1.5.7/versup/versioning.py`

 * *Files identical despite different names*

### Comparing `versup-1.5.6/PKG-INFO` & `versup-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versup
-Version: 1.5.6
+Version: 1.5.7
 Summary: Version up your project with ease.
 Home-page: https://github.com/Svenito/versup
 License: MIT
 Author: Sven Steinbauer
 Author-email: sven@unlogic.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

