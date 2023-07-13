# Comparing `tmp/aws-ssm-tool-2023.7.13.8.54.tar.gz` & `tmp/aws-ssm-tool-2023.7.13.9.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ssm-tool-2023.7.13.8.54.tar", last modified: Thu Jul 13 15:54:00 2023, max compression
+gzip compressed data, was "aws-ssm-tool-2023.7.13.9.10.tar", last modified: Thu Jul 13 16:10:04 2023, max compression
```

## Comparing `aws-ssm-tool-2023.7.13.8.54.tar` & `aws-ssm-tool-2023.7.13.9.10.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/
--rw-rw-r--   0 matt      (1000) matt      (1000)      637 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2333 2023-07-13 14:54:53.000000 aws-ssm-tool-2023.7.13.8.54/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)     1239 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      765 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.8.54/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      637 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      369 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      185 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        4 2023-07-13 15:54:00.000000 aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/top_level.txt
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 15:54:00.096243 aws-ssm-tool-2023.7.13.8.54/src/ssm/
--rw-rw-r--   0 matt      (1000) matt      (1000)       12 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.8.54/src/ssm/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       78 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.8.54/src/ssm/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-07-13 15:53:57.000000 aws-ssm-tool-2023.7.13.8.54/src/ssm/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2333 2023-07-13 14:54:53.000000 aws-ssm-tool-2023.7.13.9.10/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1276 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      765 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      369 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      206 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        4 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/ssm/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       12 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       78 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-07-13 16:10:01.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/_version.py
```

### Comparing `aws-ssm-tool-2023.7.13.8.54/PKG-INFO` & `aws-ssm-tool-2023.7.13.9.10/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.8.54
+Version: 2023.7.13.9.10
 Summary: AWS SSM tool
-Home-page: https://github.com/Robot-Wranglers/ssm-tool/
+Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
-Project-URL: Documentation, https://github.com/Robot-Wranglers/ssm-tool/
-Project-URL: Source, https://github.com/Robot-Wranglers/ssm-tool/
-Project-URL: Download, https://github.com/Robot-Wranglers/ssm-tool/#files
+Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
+Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
+Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
```

### Comparing `aws-ssm-tool-2023.7.13.8.54/README.md` & `aws-ssm-tool-2023.7.13.9.10/README.md`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.8.54/setup.cfg` & `aws-ssm-tool-2023.7.13.9.10/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 description = AWS SSM tool
 author = Robot-Wranglers
 platforms = any
 license = MIT
 license_files = LICENSE.txt
 long_description = See the project README
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/Robot-Wranglers/ssm-tool/
+url = https://github.com/Robot-Wranglers/aws-ssm-tool/
 project_urls = 
-	Documentation = https://github.com/Robot-Wranglers/ssm-tool/
-	Source = https://github.com/Robot-Wranglers/ssm-tool/
-	Download = https://github.com/Robot-Wranglers/ssm-tool/#files
+	Documentation = https://github.com/Robot-Wranglers/aws-ssm-tool/
+	Source = https://github.com/Robot-Wranglers/aws-ssm-tool/
+	Download = https://github.com/Robot-Wranglers/aws-ssm-tool/#files
 classifiers = 
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 zip_ok = False
 packages = 
@@ -39,23 +39,23 @@
 	tests
 
 [options.extras_require]
 dev = 
 	IPython
 testing = 
 	IPython
-	tox
+	tox==4.6.4
 	pytest
 	pytest-cov
 	mock
 	flake8==5.0.4
 lint = 
-	tox
+	tox==4.6.4
 publish = 
-	twine
+	twine==4.0.2
 
 [options.package_data]
 * = *.json
 
 [options.entry_points]
 console_scripts = 
 	ssm = ssm.bin.ssm:entry
```

### Comparing `aws-ssm-tool-2023.7.13.8.54/setup.py` & `aws-ssm-tool-2023.7.13.9.10/setup.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.8.54/src/aws_ssm_tool.egg-info/PKG-INFO` & `aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.8.54
+Version: 2023.7.13.9.10
 Summary: AWS SSM tool
-Home-page: https://github.com/Robot-Wranglers/ssm-tool/
+Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
-Project-URL: Documentation, https://github.com/Robot-Wranglers/ssm-tool/
-Project-URL: Source, https://github.com/Robot-Wranglers/ssm-tool/
-Project-URL: Download, https://github.com/Robot-Wranglers/ssm-tool/#files
+Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
+Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
+Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
```

