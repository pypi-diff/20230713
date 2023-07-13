# Comparing `tmp/codeboxapi-0.0.4.tar.gz` & `tmp/codeboxapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.4.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.5.tar", max compression
```

## Comparing `codeboxapi-0.0.4.tar` & `codeboxapi-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:15:22.624340 codeboxapi-0.0.4/LICENSE
--rw-r--r--   0        0        0      990 2023-07-09 10:49:25.608594 codeboxapi-0.0.4/README.md
--rw-r--r--   0        0        0      453 2023-07-08 10:18:47.139651 codeboxapi-0.0.4/codeboxapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 20:22:44.654362 codeboxapi-0.0.4/codeboxapi/chromebox.todo
--rw-r--r--   0        0        0     2939 2023-07-10 13:56:20.504620 codeboxapi-0.0.4/codeboxapi/codebox.py
--rw-r--r--   0        0        0      373 2023-07-08 09:58:38.756932 codeboxapi-0.0.4/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-06 15:43:19.461194 codeboxapi-0.0.4/codeboxapi/errors.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:56.443613 codeboxapi-0.0.4/codeboxapi/repobox.todo
--rw-r--r--   0        0        0      401 2023-07-04 21:36:12.057702 codeboxapi-0.0.4/codeboxapi/schema.py
--rw-r--r--   0        0        0      913 2023-07-08 12:34:43.495991 codeboxapi-0.0.4/codeboxapi/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:44.232581 codeboxapi-0.0.4/codeboxapi/vectorbox.todo
--rw-r--r--   0        0        0      498 2023-07-10 14:27:10.973487 codeboxapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 codeboxapi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-09 15:46:48.719311 codeboxapi-0.0.5/README.md
+-rw-r--r--   0        0        0      447 2023-07-11 16:58:07.407377 codeboxapi-0.0.5/codeboxapi/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-11 17:29:00.964544 codeboxapi-0.0.5/codeboxapi/box/__init__.py
+-rw-r--r--   0        0        0     2351 2023-07-13 21:08:10.583088 codeboxapi-0.0.5/codeboxapi/box/basebox.py
+-rw-r--r--   0        0        0     5406 2023-07-13 21:07:44.997003 codeboxapi-0.0.5/codeboxapi/box/codebox.py
+-rw-r--r--   0        0        0    15864 2023-07-13 21:03:53.020903 codeboxapi-0.0.5/codeboxapi/box/localbox.py
+-rw-r--r--   0        0        0      386 2023-07-11 16:38:34.010791 codeboxapi-0.0.5/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.5/codeboxapi/errors.py
+-rw-r--r--   0        0        0      590 2023-07-12 14:35:14.261440 codeboxapi-0.0.5/codeboxapi/schema.py
+-rw-r--r--   0        0        0     2457 2023-07-13 21:12:43.142966 codeboxapi-0.0.5/codeboxapi/utils.py
+-rw-r--r--   0        0        0      595 2023-07-13 17:41:29.816671 codeboxapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 codeboxapi-0.0.5/PKG-INFO
```

### Comparing `codeboxapi-0.0.4/LICENSE` & `codeboxapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.4/README.md` & `codeboxapi-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 
 # print the result
 print(result)
 
 codebox.stop()
 ```
 
+## Where to get your api-key?
+
+CodeBox is currently in early development just write me an email and I send you a key for testing :)
+
+
 ## Contributing
 
 Feel free to contribute to this project.
 You can open an issue or submit a pull request.
 
 ## License
```

### Comparing `codeboxapi-0.0.4/codeboxapi/errors.py` & `codeboxapi-0.0.5/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.4/PKG-INFO` & `codeboxapi-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: codeboxapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 # CodeBox
 
 CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 It allows you to run python code in an isolated/sandboxed environment.
 Additionally, it provides simple fileIO (and vector database support coming soon).
@@ -50,14 +53,19 @@
 
 # print the result
 print(result)
 
 codebox.stop()
 ```
 
+## Where to get your api-key?
+
+CodeBox is currently in early development just write me an email and I send you a key for testing :)
+
+
 ## Contributing
 
 Feel free to contribute to this project.
 You can open an issue or submit a pull request.
 
 ## License
```

