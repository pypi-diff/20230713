# Comparing `tmp/aws-ssm-tool-2023.7.13.9.10.tar.gz` & `tmp/aws-ssm-tool-2023.7.13.9.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ssm-tool-2023.7.13.9.10.tar", last modified: Thu Jul 13 16:10:04 2023, max compression
+gzip compressed data, was "aws-ssm-tool-2023.7.13.9.24.tar", last modified: Thu Jul 13 16:24:37 2023, max compression
```

## Comparing `aws-ssm-tool-2023.7.13.9.10.tar` & `aws-ssm-tool-2023.7.13.9.24.tar`

### file list

```diff
@@ -1,18 +1,35 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/
--rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2333 2023-07-13 14:54:53.000000 aws-ssm-tool-2023.7.13.9.10/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)     1276 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      765 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      369 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      206 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        4 2023-07-13 16:10:04.000000 aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/top_level.txt
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:10:04.682474 aws-ssm-tool-2023.7.13.9.10/src/ssm/
--rw-rw-r--   0 matt      (1000) matt      (1000)       12 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       78 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-07-13 16:10:01.000000 aws-ssm-tool-2023.7.13.9.10/src/ssm/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2333 2023-07-13 14:54:53.000000 aws-ssm-tool-2023.7.13.9.24/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1278 2023-07-13 16:24:37.797945 aws-ssm-tool-2023.7.13.9.24/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      765 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.789945 aws-ssm-tool-2023.7.13.9.24/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      653 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      651 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      206 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        4 2023-07-13 16:24:37.000000 aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       12 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       78 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-07-13 16:24:35.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       97 2023-07-13 16:21:21.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      506 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/abcs/loggable.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4086 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5528 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/environment.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2879 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/api/manager.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2662 2023-07-13 16:22:40.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/bin/ssm.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1578 2023-07-13 16:23:49.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/args.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5037 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3640 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/cli/wrapper.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-13 16:24:37.793945 aws-ssm-tool-2023.7.13.9.24/src/ssm/util/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1784 2023-07-13 15:47:55.000000 aws-ssm-tool-2023.7.13.9.24/src/ssm/util/__init__.py
```

### Comparing `aws-ssm-tool-2023.7.13.9.10/PKG-INFO` & `aws-ssm-tool-2023.7.13.9.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.9.10
+Version: 2023.7.13.9.24
 Summary: AWS SSM tool
 Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
 Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
```

### Comparing `aws-ssm-tool-2023.7.13.9.10/README.md` & `aws-ssm-tool-2023.7.13.9.24/README.md`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.10/setup.cfg` & `aws-ssm-tool-2023.7.13.9.24/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 classifiers = 
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 zip_ok = False
 packages = 
-	ssm
+	find:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >3.7
 install_requires = 
 	click
 	pyyaml
```

### Comparing `aws-ssm-tool-2023.7.13.9.10/setup.py` & `aws-ssm-tool-2023.7.13.9.24/setup.py`

 * *Files identical despite different names*

### Comparing `aws-ssm-tool-2023.7.13.9.10/src/aws_ssm_tool.egg-info/PKG-INFO` & `aws-ssm-tool-2023.7.13.9.24/src/aws_ssm_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-tool
-Version: 2023.7.13.9.10
+Version: 2023.7.13.9.24
 Summary: AWS SSM tool
 Home-page: https://github.com/Robot-Wranglers/aws-ssm-tool/
 Author: Robot-Wranglers
 License: MIT
 Project-URL: Documentation, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Source, https://github.com/Robot-Wranglers/aws-ssm-tool/
 Project-URL: Download, https://github.com/Robot-Wranglers/aws-ssm-tool/#files
```

