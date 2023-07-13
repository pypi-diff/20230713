# Comparing `tmp/py-datalab-0.2.3.tar.gz` & `tmp/py-datalab-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-datalab-0.2.3.tar", last modified: Tue Jul 11 08:40:23 2023, max compression
+gzip compressed data, was "py-datalab-0.2.4.tar", last modified: Thu Jul 13 09:39:21 2023, max compression
```

## Comparing `py-datalab-0.2.3.tar` & `py-datalab-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.111597 py-datalab-0.2.3/
--rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      802 2023-07-11 08:40:23.109590 py-datalab-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.083366 py-datalab-0.2.3/datalab/
--rw-rw-rw-   0        0        0    27910 2023-07-11 08:39:26.000000 py-datalab-0.2.3/datalab/Matrix.py
--rw-rw-rw-   0        0        0    12648 2023-07-07 15:11:17.000000 py-datalab-0.2.3/datalab/Vector.py
--rw-rw-rw-   0        0        0      204 2023-07-07 17:04:55.000000 py-datalab-0.2.3/datalab/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.3/datalab/functions.py
--rw-rw-rw-   0        0        0     2110 2023-07-11 06:36:46.000000 py-datalab-0.2.3/datalab/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:40:23.107085 py-datalab-0.2.3/py_datalab.egg-info/
--rw-rw-rw-   0        0        0      802 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 08:40:22.000000 py-datalab-0.2.3/py_datalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 08:40:23.111597 py-datalab-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1059 2023-07-11 08:39:53.000000 py-datalab-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:39:21.023762 py-datalab-0.2.4/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 10:54:28.000000 py-datalab-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      846 2023-07-13 09:39:21.022761 py-datalab-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2023-07-07 04:02:41.000000 py-datalab-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 09:39:21.007264 py-datalab-0.2.4/datalab/
+-rw-rw-rw-   0        0        0    27910 2023-07-11 08:39:26.000000 py-datalab-0.2.4/datalab/Matrix.py
+-rw-rw-rw-   0        0        0    21914 2023-07-13 09:32:38.000000 py-datalab-0.2.4/datalab/Vector.py
+-rw-rw-rw-   0        0        0      204 2023-07-07 17:04:55.000000 py-datalab-0.2.4/datalab/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-07-07 16:59:02.000000 py-datalab-0.2.4/datalab/functions.py
+-rw-rw-rw-   0        0        0     2110 2023-07-11 06:36:46.000000 py-datalab-0.2.4/datalab/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:39:21.021762 py-datalab-0.2.4/py_datalab.egg-info/
+-rw-rw-rw-   0        0        0      846 2023-07-13 09:39:20.000000 py-datalab-0.2.4/py_datalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-07-13 09:39:20.000000 py-datalab-0.2.4/py_datalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:39:20.000000 py-datalab-0.2.4/py_datalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-13 09:39:20.000000 py-datalab-0.2.4/py_datalab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 09:39:20.000000 py-datalab-0.2.4/py_datalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:39:21.023762 py-datalab-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1102 2023-07-13 09:39:06.000000 py-datalab-0.2.4/setup.py
```

### Comparing `py-datalab-0.2.3/LICENSE` & `py-datalab-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.3/PKG-INFO` & `py-datalab-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.3
+Version: 0.2.4
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
```

### Comparing `py-datalab-0.2.3/README.md` & `py-datalab-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.3/datalab/Matrix.py` & `py-datalab-0.2.4/datalab/Matrix.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.3/datalab/functions.py` & `py-datalab-0.2.4/datalab/functions.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.3/datalab/utils.py` & `py-datalab-0.2.4/datalab/utils.py`

 * *Files identical despite different names*

### Comparing `py-datalab-0.2.3/py_datalab.egg-info/PKG-INFO` & `py-datalab-0.2.4/py_datalab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: py-datalab
-Version: 0.2.3
+Version: 0.2.4
 Summary: This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.
 Home-page: https://github.com/matuszen/Python-DataLab
 Author: Mateusz Nowak
 Author-email: mateusz.nowak.pol@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
```

### Comparing `py-datalab-0.2.3/setup.py` & `py-datalab-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 10):
     sys.exit("Sorry, Python < 3.10 is not supported")
 
 setup(
     name="py-datalab",
-    version="0.2.3",
+    version="0.2.4",
     author="Mateusz Nowak",
     author_email="mateusz.nowak.pol@gmail.com",
     description="This project provides classes for working with data in python. Actually there are two classes: Matrix and Vector.",
     url="https://github.com/matuszen/Python-DataLab",
     packages=find_packages(),
     install_requires=[
         "typing_extensions",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3 :: Only",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
     ],
 )
```

