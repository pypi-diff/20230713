# Comparing `tmp/searchy-1.0.0.tar.gz` & `tmp/searchy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchy-1.0.0.tar", last modified: Wed Jul 12 18:23:04 2023, max compression
+gzip compressed data, was "searchy-1.0.1.tar", last modified: Wed Jul 12 18:36:46 2023, max compression
```

## Comparing `searchy-1.0.0.tar` & `searchy-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:23:04.557557 searchy-1.0.0/
--rw-r--r--   0 lactua    (1000) lactua    (1000)      381 2023-07-12 18:23:04.557557 searchy-1.0.0/PKG-INFO
--rw-r--r--   0 lactua    (1000) lactua    (1000)       38 2023-07-12 18:23:04.557557 searchy-1.0.0/setup.cfg
--rw-r--r--   0 lactua    (1000) lactua    (1000)      609 2023-07-12 18:21:03.000000 searchy-1.0.0/setup.py
-drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:23:04.557557 searchy-1.0.0/src/
-drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:23:04.557557 searchy-1.0.0/src/searchy/
--rw-r--r--   0 lactua    (1000) lactua    (1000)     1055 2023-07-12 18:15:17.000000 searchy-1.0.0/src/searchy/__init__.py
-drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:23:04.557557 searchy-1.0.0/src/searchy.egg-info/
--rw-r--r--   0 lactua    (1000) lactua    (1000)      381 2023-07-12 18:23:04.000000 searchy-1.0.0/src/searchy.egg-info/PKG-INFO
--rw-r--r--   0 lactua    (1000) lactua    (1000)      206 2023-07-12 18:23:04.000000 searchy-1.0.0/src/searchy.egg-info/SOURCES.txt
--rw-r--r--   0 lactua    (1000) lactua    (1000)        1 2023-07-12 18:23:04.000000 searchy-1.0.0/src/searchy.egg-info/dependency_links.txt
--rw-r--r--   0 lactua    (1000) lactua    (1000)        7 2023-07-12 18:23:04.000000 searchy-1.0.0/src/searchy.egg-info/requires.txt
--rw-r--r--   0 lactua    (1000) lactua    (1000)        8 2023-07-12 18:23:04.000000 searchy-1.0.0/src/searchy.egg-info/top_level.txt
+drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:36:46.638436 searchy-1.0.1/
+-rw-r--r--   0 lactua    (1000) lactua    (1000)      381 2023-07-12 18:36:46.638436 searchy-1.0.1/PKG-INFO
+-rw-r--r--   0 lactua    (1000) lactua    (1000)       38 2023-07-12 18:36:46.638436 searchy-1.0.1/setup.cfg
+-rw-r--r--   0 lactua    (1000) lactua    (1000)      710 2023-07-12 18:36:41.000000 searchy-1.0.1/setup.py
+drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:36:46.638436 searchy-1.0.1/src/
+drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:36:46.638436 searchy-1.0.1/src/searchy/
+-rw-r--r--   0 lactua    (1000) lactua    (1000)     1082 2023-07-12 18:33:54.000000 searchy-1.0.1/src/searchy/__init__.py
+drwxr-xr-x   0 lactua    (1000) lactua    (1000)        0 2023-07-12 18:36:46.638436 searchy-1.0.1/src/searchy.egg-info/
+-rw-r--r--   0 lactua    (1000) lactua    (1000)      381 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/PKG-INFO
+-rw-r--r--   0 lactua    (1000) lactua    (1000)      244 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/SOURCES.txt
+-rw-r--r--   0 lactua    (1000) lactua    (1000)        1 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/dependency_links.txt
+-rw-r--r--   0 lactua    (1000) lactua    (1000)       41 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/entry_points.txt
+-rw-r--r--   0 lactua    (1000) lactua    (1000)        7 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/requires.txt
+-rw-r--r--   0 lactua    (1000) lactua    (1000)        8 2023-07-12 18:36:46.000000 searchy-1.0.1/src/searchy.egg-info/top_level.txt
```

### Comparing `searchy-1.0.0/setup.py` & `searchy-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import setuptools
 
 setuptools.setup(
     name="searchy",
-    version="1.0.0",
+    version="1.0.1",
     author="lactua",
     author_email="lactua@lactua.com",
     description="Python package that allows you to search on google from commands",
     long_description="",
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=['google'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
+    entry_points={
+        'console_scripts': [
+            'searchy = searchy:main'
+        ]
+    }
 )
```

### Comparing `searchy-1.0.0/src/searchy/__init__.py` & `searchy-1.0.1/src/searchy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 
     for arg in args:
         argument_parser.add_argument(arg[0], **arg[1])
 
     input_args = argument_parser.parse_args().__dict__
     return input_args
 
+def main():
+    args = parseArguments(*ARGS)
 
-args = parseArguments(*ARGS)
+    results = search(**args)
 
-results = search(**args)
-
-for index in range(args['num']):
-    print(f'{index+1}. {next(results)}')
+    for index in range(args['num']):
+        print(f'{index+1}. {next(results)}')
```

