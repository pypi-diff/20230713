# Comparing `tmp/rizallogger-0.1.tar.gz` & `tmp/rizallogger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rizallogger-0.1.tar", last modified: Thu Jul 13 05:40:53 2023, max compression
+gzip compressed data, was "rizallogger-0.2.tar", last modified: Thu Jul 13 06:03:20 2023, max compression
```

## Comparing `rizallogger-0.1.tar` & `rizallogger-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 05:40:53.124570 rizallogger-0.1/
--rw-rw-rw-   0        0        0     1086 2023-07-13 02:42:52.000000 rizallogger-0.1/LICENSE
--rw-rw-rw-   0        0        0      740 2023-07-13 05:40:53.124570 rizallogger-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-13 03:27:23.000000 rizallogger-0.1/README.md
--rw-rw-rw-   0        0        0      302 2023-07-13 02:55:42.000000 rizallogger-0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-13 05:40:53.108279 rizallogger-0.1/rizallogger/
--rw-rw-rw-   0        0        0      985 2023-07-13 03:11:53.000000 rizallogger-0.1/rizallogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 05:40:53.124570 rizallogger-0.1/rizallogger.egg-info/
--rw-rw-rw-   0        0        0      740 2023-07-13 05:40:53.000000 rizallogger-0.1/rizallogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-13 05:40:53.000000 rizallogger-0.1/rizallogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 05:40:53.000000 rizallogger-0.1/rizallogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-13 05:40:53.000000 rizallogger-0.1/rizallogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-13 05:40:53.124570 rizallogger-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-07-13 05:40:15.000000 rizallogger-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:03:20.487138 rizallogger-0.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-13 02:42:52.000000 rizallogger-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1073 2023-07-13 06:03:20.487138 rizallogger-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-13 03:27:23.000000 rizallogger-0.2/README.md
+-rw-rw-rw-   0        0        0      302 2023-07-13 02:55:42.000000 rizallogger-0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-13 06:03:20.477906 rizallogger-0.2/rizallogger/
+-rw-rw-rw-   0        0        0      985 2023-07-13 03:11:53.000000 rizallogger-0.2/rizallogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:03:20.487138 rizallogger-0.2/rizallogger.egg-info/
+-rw-rw-rw-   0        0        0     1073 2023-07-13 06:03:20.000000 rizallogger-0.2/rizallogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-13 06:03:20.000000 rizallogger-0.2/rizallogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:03:20.000000 rizallogger-0.2/rizallogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 06:03:20.000000 rizallogger-0.2/rizallogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-13 06:03:20.494176 rizallogger-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2023-07-13 06:02:38.000000 rizallogger-0.2/setup.py
```

### Comparing `rizallogger-0.1/LICENSE` & `rizallogger-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rizallogger-0.1/PKG-INFO` & `rizallogger-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rizallogger
-Version: 0.1
+Version: 0.2
 Summary: Make easy to log your project
 Home-page: https://github.com/rzmobiledev/rzlogger
 Download-URL: https://github.com/rzmobiledev/rzlogger/archive/v_01.tar.gz
 Author: Safrizal
 Author-email: rzmobiledev@gmail.com
 License: MIT
 Keywords: rzlogger,easylog,rizallogger,rz-logger
@@ -13,7 +13,24 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires: logging
 License-File: LICENSE
+
+# RZLogger
+
+Make easy to log all your projects
+
+## Set up for local development
+
+- if you don't have pip installed, install it first
+- run `pip install rzlogger`
+
+## Import and use the logger
+
+Now you can use the logger by accessing the class `Log`.
+
+`from rzlogger import Log`
+`Log.warning('your error message')`
+
```

### Comparing `rizallogger-0.1/rizallogger/__init__.py` & `rizallogger-0.2/rizallogger/__init__.py`

 * *Files identical despite different names*

### Comparing `rizallogger-0.1/rizallogger.egg-info/PKG-INFO` & `rizallogger-0.2/rizallogger.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rizallogger
-Version: 0.1
+Version: 0.2
 Summary: Make easy to log your project
 Home-page: https://github.com/rzmobiledev/rzlogger
 Download-URL: https://github.com/rzmobiledev/rzlogger/archive/v_01.tar.gz
 Author: Safrizal
 Author-email: rzmobiledev@gmail.com
 License: MIT
 Keywords: rzlogger,easylog,rizallogger,rz-logger
@@ -13,7 +13,24 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires: logging
 License-File: LICENSE
+
+# RZLogger
+
+Make easy to log all your projects
+
+## Set up for local development
+
+- if you don't have pip installed, install it first
+- run `pip install rzlogger`
+
+## Import and use the logger
+
+Now you can use the logger by accessing the class `Log`.
+
+`from rzlogger import Log`
+`Log.warning('your error message')`
+
```

### Comparing `rizallogger-0.1/setup.py` & `rizallogger-0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from pathlib import Path
 from distutils.core import setup
 
+directory = Path(__file__).parent
+
 setup(
     name="rizallogger",
     packages=["rizallogger"],
-    version="0.1",
+    version="0.2",
     license="MIT",
     description="Make easy to log your project",
+    long_description=(directory / "README.md").read_text(),
     author="Safrizal",
     author_email="rzmobiledev@gmail.com",
     url="https://github.com/rzmobiledev/rzlogger",
     download_url="https://github.com/rzmobiledev/rzlogger/archive/v_01.tar.gz",
     keywords=["rzlogger", "easylog", "rizallogger", "rz-logger"],
     # package need to install / package used in this package
     requires=["logging"],
```

