# Comparing `tmp/f5project-0.0.8.tar.gz` & `tmp/f5project-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f5project-0.0.8.tar", last modified: Thu Jul 13 03:07:06 2023, max compression
+gzip compressed data, was "f5project-0.0.9.tar", last modified: Thu Jul 13 03:09:20 2023, max compression
```

## Comparing `f5project-0.0.8.tar` & `f5project-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:07:06.274407 f5project-0.0.8/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-07-11 00:45:10.000000 f5project-0.0.8/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 03:07:06.274269 f5project-0.0.8/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     6646 2023-07-11 00:45:10.000000 f5project-0.0.8/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:07:06.273121 f5project-0.0.8/f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)    11852 2023-07-13 02:44:43.000000 f5project-0.0.8/f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:07:06.273997 f5project-0.0.8/f5project/create_f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)      634 2023-07-13 02:44:43.000000 f5project-0.0.8/f5project/create_f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:07:06.273869 f5project-0.0.8/f5project.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      287 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       65 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/entry_points.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/requires.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-13 03:07:06.000000 f5project-0.0.8/f5project.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-13 03:07:06.274454 f5project-0.0.8/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      922 2023-07-13 03:06:49.000000 f5project-0.0.8/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:09:20.320433 f5project-0.0.9/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-07-11 00:45:10.000000 f5project-0.0.9/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 03:09:20.320296 f5project-0.0.9/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     6646 2023-07-11 00:45:10.000000 f5project-0.0.9/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:09:20.319324 f5project-0.0.9/f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)    11852 2023-07-13 02:44:43.000000 f5project-0.0.9/f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:09:20.319445 f5project-0.0.9/f5project/create_f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)      634 2023-07-13 02:44:43.000000 f5project-0.0.9/f5project/create_f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-13 03:09:20.320070 f5project-0.0.9/f5project.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     7095 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      291 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       65 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/entry_points.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/requires.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-13 03:09:20.000000 f5project-0.0.9/f5project.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-13 03:09:20.320478 f5project-0.0.9/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      949 2023-07-13 03:09:10.000000 f5project-0.0.9/setup.py
```

### Comparing `f5project-0.0.8/LICENSE` & `f5project-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `f5project-0.0.8/PKG-INFO` & `f5project-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5project
-Version: 0.0.8
+Version: 0.0.9
 Summary: F5 project
 Home-page: https://github.com/thejimmylin/f5project
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f5project-0.0.8/README.md` & `f5project-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `f5project-0.0.8/f5project/__init__.py` & `f5project-0.0.9/f5project/__init__.py`

 * *Files identical despite different names*

### Comparing `f5project-0.0.8/f5project/create_f5project/__init__.py` & `f5project-0.0.9/f5project/create_f5project/__init__.py`

 * *Files identical despite different names*

### Comparing `f5project-0.0.8/f5project.egg-info/PKG-INFO` & `f5project-0.0.9/f5project.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5project
-Version: 0.0.8
+Version: 0.0.9
 Summary: F5 project
 Home-page: https://github.com/thejimmylin/f5project
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `f5project-0.0.8/setup.py` & `f5project-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 
 setuptools.setup(
     name="f5project",
-    version="0.0.8",
+    version="0.0.9",
     install_requires=[
         "github-secret-syncer",
     ],
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="F5 project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/f5project",
     packages=setuptools.find_packages(),
+    package_dir={"": "."},
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "create-f5project = f5project:create_f5project",
         ],
     },
     classifiers=[
```

