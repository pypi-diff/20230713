# Comparing `tmp/mauritstestpackage2-3.0.0a16.tar.gz` & `tmp/mauritstestpackage2-3.0.0a17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauritstestpackage2-3.0.0a16.tar", last modified: Wed Jul 12 21:49:28 2023, max compression
+gzip compressed data, was "mauritstestpackage2-3.0.0a17.tar", last modified: Thu Jul 13 12:46:30 2023, max compression
```

## Comparing `mauritstestpackage2-3.0.0a16.tar` & `mauritstestpackage2-3.0.0a17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.355840 mauritstestpackage2-3.0.0a16/
--rw-r--r--   0 maurits    (501) staff       (20)     4527 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5321 2023-07-12 21:49:28.355969 mauritstestpackage2-3.0.0a16/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.353927 mauritstestpackage2-3.0.0a16/mauritstestpackage/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.351968 mauritstestpackage2-3.0.0a16/mauritstestpackage/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.352063 mauritstestpackage2-3.0.0a16/mauritstestpackage/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.354213 mauritstestpackage2-3.0.0a16/mauritstestpackage/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-12 21:49:28.355600 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     5321 2023-07-12 21:49:28.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-12 21:49:28.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 21:49:28.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-12 21:49:28.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       19 2023-07-12 21:49:28.000000 mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-12 21:49:28.356436 mauritstestpackage2-3.0.0a16/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-07-12 21:49:27.000000 mauritstestpackage2-3.0.0a16/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.320341 mauritstestpackage2-3.0.0a17/
+-rw-r--r--   0 maurits    (501) staff       (20)     4597 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5317 2023-07-13 12:46:30.320476 mauritstestpackage2-3.0.0a17/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.318371 mauritstestpackage2-3.0.0a17/mauritstestpackage/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.316653 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.316727 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.318592 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 12:46:30.320005 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5317 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-07-13 12:46:30.000000 mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-13 12:46:30.320827 mauritstestpackage2-3.0.0a17/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-07-13 12:46:29.000000 mauritstestpackage2-3.0.0a17/setup.py
```

### Comparing `mauritstestpackage2-3.0.0a16/CHANGES.rst` & `mauritstestpackage2-3.0.0a17/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+3.0.0a17 (2023-07-13)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a16 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a15 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a16/PKG-INFO` & `mauritstestpackage2-3.0.0a17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a16
+Version: 3.0.0a17
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 
 Test package.
 
 I can use this for testing zest.releaser upload to PyPI.
 
 Or testpypi.
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.0a17 (2023-07-13)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a16 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a15 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a16/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po` & `mauritstestpackage2-3.0.0a17/mauritstestpackage/locales/nl/LC_MESSAGES/mauritstestpackage.po`

 * *Files identical despite different names*

### Comparing `mauritstestpackage2-3.0.0a16/mauritstestpackage2.egg-info/PKG-INFO` & `mauritstestpackage2-3.0.0a17/mauritstestpackage2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: mauritstestpackage2
-Version: 3.0.0a16
+Version: 3.0.0a17
 Summary: Test package from Maurits for uploading to PyPI.
 Home-page: https://github.com/mauritsvanrees/mauritstestpackage
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: test release pypi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 
 Test package.
 
 I can use this for testing zest.releaser upload to PyPI.
 
 Or testpypi.
 
 Maurits van Rees
 
 
 Changelog
 =========
 
+3.0.0a17 (2023-07-13)
+---------------------
+
+- Nothing changed yet.
+
+
 3.0.0a16 (2023-07-12)
 ---------------------
 
 - Nothing changed yet.
 
 
 3.0.0a15 (2023-07-12)
```

### Comparing `mauritstestpackage2-3.0.0a16/setup.py` & `mauritstestpackage2-3.0.0a17/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import setup, find_packages
+from setuptools import find_namespace_packages
+from setuptools import setup
 
-version = "3.0.0a16"
+
+version = "3.0.0a17"
 
 setup(
     name="mauritstestpackage2",
     version=version,
     description="Test package from Maurits for uploading to PyPI.",
     long_description=(open("README.rst").read() + "\n\n" + open("CHANGES.rst").read()),
     # Get strings from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="test release pypi",
     author="Maurits van Rees",
     author_email="maurits@vanrees.org",
     url="https://github.com/mauritsvanrees/mauritstestpackage",
     license="GPL",
-    packages=find_packages(exclude=["ez_setup", "examples", "tests"]),
+    packages=find_namespace_packages(),
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        # -*- Extra requirements: -*-
     ],
     entry_points="""
       # -*- Entry points: -*-
       """,
 )
```

